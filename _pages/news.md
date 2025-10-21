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
        /* Instagram gallery grid */
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
    <!-- Instagram Gallery -->
    <div class="image-grid">
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7384599261256048640?collapsed=1" height="603" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>
        <iframe src="https://www.linkedin.com/posts/marjhum-akter_attended-an-impactful-seminar-on-bioinformatics-activity-7361744320892194817-4o7O?utm_source=share&utm_medium=member_desktop&rcm=ACoAAA0Nx6EBI3OYbgGUoYJqLq9hv7LBwpedIPs" height="603" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7339221163610443777?collapsed=1" height="669" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>
        <iframe src="https://www.linkedin.com/embed/feed/update/urn:li:share:7325068183889936384?collapsed=1" height="627" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>
    </div>
    <!-- Twitter Embed -->
    <div class="twitter-embed">
        <blockquote class="twitter-tweet"><p lang="en" dir="ltr">SLU&#39;s day of Bioinformatics,<br>lovely gathering, talks and discussions!!<a href="https://twitter.com/PlantSlu?ref_src=twsrc%5Etfw">@PlantSlu</a> <a href="https://twitter.com/SLUpostdocs?ref_src=twsrc%5Etfw">@SLUpostdocs</a> <a href="https://t.co/3Cn4RFb98v">pic.twitter.com/3Cn4RFb98v</a></p>&mdash; Abu B Siddique (@absiddique85) <a href="https://twitter.com/absiddique85/status/1706304748926685625?ref_src=twsrc%5Etfw">September 25, 2023</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
    </div>
</div>

</body>
