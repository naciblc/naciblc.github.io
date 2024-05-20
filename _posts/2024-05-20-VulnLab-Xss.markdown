---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Yavuzlar_Vuln_xss_sql
title: Yavuzlar Vulnlab Xss Sql İnjection Çözümüleri

# post specific
# if not specified, .name will be used from _data/owner.yml
author: Naci Balcı
# multiple category is not supported
category: Vulnlab
# multiple tag entries are possible
tags: [Xss, Sql Injection]
# thumbnail image for post
img: ":yavuzlar.png"
# disable comments on this page
#comments_disable: true

# publish date
date: 2024-05-20 12:32:10 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-03-03 12:32:10 +0900
# check the meta_common_description in _data/lang/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LinkedIn PDF Viewer</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #2c3e50; /* Arka plan rengini değiştirdim */
        }
        iframe {
            width: 90%;
            height: 95%;
            border: none; /* Kenarlıkları kaldırdım */
        }
    </style>
</head>
<body>
    <iframe src="https://drive.google.com/file/d/1dciAJ0KGGBm62zF7JJpDttw1KmnEbnEj/preview" frameborder="0"></iframe>
</body>
