---
layout: single
permalink: /news/
author_profile: true
classes: wide
---

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>News - Responsive Layout</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        /* Container for the whole layout */
        .container {
            display: flex;
            justify-content: space-between;
            align-items: flex-start; /* Align items at the top */
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            box-sizing: border-box;
        }
        /* Linkedin gallery grid */
        .image-grid {
            flex-basis: 60%; /* Image section takes up 60% of the container width */
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-gap: 5px;
        }
        .image-grid img {
            width: 100%;
            height: auto;
            object-fit: cover;
        }
        /* Twitter embed section */
        .twitter-embed {
            flex-basis: 40%; /* Twitter section takes up 35% of the container width */
            margin-left: 1%;
        }
        /* For smaller screens (max-width: 1024px) */
        @media (max-width: 1024px) {
            .container {
                flex-wrap: wrap;
            }
            .image-grid {
                flex-basis: 100%; /* Image grid takes full width */
                grid-template-columns: repeat(3, 1fr);
            }
            .twitter-embed {
                flex-basis: 100%; /* Twitter embed takes full width */
                margin-top: 20px; /* Add margin to separate from images */
            }
        }
        /* For mobile screens (max-width: 768px) */
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
                align-items: center;
            }
            .image-grid {
                grid-template-columns: repeat(3, 1fr);
            }
            .twitter-embed {
                width: 100%; /* Full width for Twitter embed */
                margin-top: 20px;
            }
        }
    </style>
</head>
<body>

<div class="container">
    <!-- Linkedin & Facebook Gallery -->    
    <div style="display: flex; flex-direction: column; gap: 20px;">
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2FTheDhakaDiary%2Fposts%2Fpfbid02XhN7noaFthVpKfCFHkSG5R3c7v2rDA5WoghM37nZYgS5uE6TFKbtLjZayr5pVENml&show_text=true&width=500" width="500" height="609" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fsaucc.org%2Fposts%2Fpfbid0ahmg7ofhDKZG2S1PtqNKGdm5pNNJmKQ65ftZKsKJA8J3jf81NnoZqsgpusv8RfHAl&show_text=true&width=500" width="500" height="792" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7386715129901469696" height="1177" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fa.b.s.biplob%2Fposts%2Fpfbid035v9CoBimjZkwaJaC6JMwEMUeGftdqn65qf5xCGY7PGhz72h8fpvme5bVKnLCXJitl&show_text=true&width=500" width="500" height="805" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7384599261256048640?collapsed=1" height="603" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe> 
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fa.b.s.biplob%2Fposts%2Fpfbid0SB2XPAbdqXWxw11HfXw1VFRFjkxqftRPa7cifkbgj6EBHyXqDPxGHcq5apSE3iT3l&show_text=true&width=500" width="500" height="667" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fa.b.s.biplob%2Fposts%2Fpfbid02aT7YisWjX9WRatFh68SrWD3RMBwNiGmFjD1nC5uS8gby38xsh5S33pXzdmU99qxol&show_text=true&width=500" width="500" height="607" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fa.b.s.biplob%2Fposts%2Fpfbid02w7FuULiAfNcSuPQDUXdaYva84zD7ioaF3ePfbSLxH86HjZmw1tL27LRCMGK4r7aql&show_text=true&width=500" width="500" height="520" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fa.b.s.biplob%2Fposts%2Fpfbid02541sZPCP3W67LUoVgZg1ZawPMs8KeeiFNSuF2YzaobjPuewHU3EWqjuiizqeeuKYl&show_text=true&width=500" width="500" height="483" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.facebook.com/plugins/post.php?href=https%3A%2F%2Fwww.facebook.com%2Fa.b.s.biplob%2Fposts%2Fpfbid02PNrCSyv9n9PAjqsUBPP81FG6cgDpPgj5cLLnfdhcr5gMDteBKLM9ae4r4LHeJU4ml&show_text=true&width=500" width="500" height="753" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share"></iframe>
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7339221163610443777?collapsed=1" height="669" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe> 
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7314915376692178944?collapsed=1" height="669" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe> 
    </div>
    <!-- Twitter Embed -->
    <div class="twitter-embed">
        <blockquote class="twitter-tweet"><p lang="en" dir="ltr">SLU&#39;s day of Bioinformatics,<br>lovely gathering, talks and discussions!!<a href="https://twitter.com/PlantSlu?ref_src=twsrc%5Etfw">@PlantSlu</a> <a href="https://twitter.com/SLUpostdocs?ref_src=twsrc%5Etfw">@SLUpostdocs</a> <a href="https://t.co/3Cn4RFb98v">pic.twitter.com/3Cn4RFb98v</a></p>&mdash; Abu B Siddique (@absiddique85) <a href="https://twitter.com/absiddique85/status/1706304748926685625?ref_src=twsrc%5Etfw">September 25, 2023</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
    </div>
</div>
