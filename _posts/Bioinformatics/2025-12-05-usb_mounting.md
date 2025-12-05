---
layout: single
title: "[Exploration] AI tools: NotebookLM vs Napkin ai"
categories: Exploration
tags: [usb, mounting, bioinformatics, WSL, linux, windows, data transfer, server, scp, troubleshooting, guide, tutorial, ]
header:
  teaser: /images/thumnail/usb.jpeg
---

# Mounting an External USB Drive in WSL and Downloading Data from a Server: My Journey

## Introduction
Working with WSL (Windows Subsystem for Linux) is convenient for Linux workflows on Windows, but mounting external USB drives can be confusing. Recently, I needed to download large datasets from a remote SLU server directly to my USB drive. What seemed simple turned into a learning experience. Here’s the full story, including the problems I faced and the step-by-step solution.

---

## The Problem
I plugged in my USB drive (**karima-cz**) and expected it to show up in WSL using:
```bash
lsblk
```
But here’s what I saw:
```
NAME MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS
sda    8:0    0 388.6M  1 disk
sdb    8:16   0   186M  1 disk
sdc    8:32   0     2G  0 disk [SWAP]
sdd    8:48   0     1T  0 disk /mnt/wslg/distro
```
No sign of my USB drive.

I checked kernel logs:
```bash
dmesg | tail -n 20
```
Output:
```
mount error: could not resolve address for vbsg-bio1.vbsg.slu.se: Unknown error
mount point does not exist.
WSL ERROR: Processing /etc/fstab with mount -a failed.
```
No USB detection messages—only WSL-related errors.

At this point, I realized:
- WSL does **not automatically mount physical USB drives** like Linux does.
- It only mounts Windows drives under `/mnt/` if configured.

---

## The Solution
Here’s what worked for me:

### ✅ Step 1: Verify USB in Windows
- Open **File Explorer** → Confirm the USB drive appears (mine was `D:`).

### ✅ Step 2: Check WSL Mount Points
Inside WSL:
```bash
ls /mnt/
```
No `d` folder → automatic mounting was disabled.

### ✅ Step 3: Create Mount Point
```bash
sudo mkdir -p /mnt/d
```

### ✅ Step 4: Manually Mount the USB
Use `drvfs` to mount the Windows drive:
```bash
sudo mount -t drvfs D: /mnt/d
```
Now:
```bash
ls /mnt/d
```
✅ USB contents visible!

### ✅ Step 5: Download Data from Server
Use `scp`:
```bash
scp username@hpc:/path/to/data /mnt/d/
```
Example:
```bash
scp bioinf4@hpc:/data/project/* /mnt/d/
```

### ✅ Step 6: Optional – Enable Auto-Mount
Edit WSL config:
```bash
sudo nano /etc/wsl.conf
```
Add:
```
[automount]
enabled = true
root = /mnt/
options = "metadata"
```
Restart WSL from PowerShell:
```powershell
wsl --shutdown
wsl
```

---

## Key Issues & Fixes
- **Issue:** USB not detected in `lsblk` → WSL doesn’t handle raw USB devices.
- **Fix:** Mount Windows drive using `drvfs`.
- **Issue:** `wsl --shutdown` failed inside WSL → Must run in PowerShell.
- **Fix:** Restart WSL from Windows, not Linux.

---

## Conclusion
If you’re using WSL and need to access an external USB drive, don’t panic if `lsblk` shows nothing. Just mount the Windows drive manually using `drvfs`. This method works perfectly for transferring large datasets from remote servers directly to your USB.

---

**Pro Tip:** If you need full Linux control over USB (e.g., raw device access), use WSL 2 with `--mount` or a native Linux system.
