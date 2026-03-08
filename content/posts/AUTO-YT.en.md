---
title: "AUTO-YT"
date: 2024-01-12T00:00:00Z
description: "An automated system to generate YouTube content using the Google API and scraping."
draft: false
---

![AUTOYT](/PersonalWEB2.0/images/auto-yt.png)

I wanted to explore **YouTube monetization** by creating an automated channel. Using the **Google YouTube API** and some **scraping** techniques, I managed to generate content in minutes without manual editing or content hunting.

---

## How does it work?

To run the system correctly, you need:

- **Instagram account credentials** to fetch videos from followed accounts.
- Access to the **Google account** of the channel where videos will be uploaded.
- A **developer account** for authentication.

The program stores uploaded video IDs in a database. When it looks for new videos, it checks whether they were uploaded before to avoid duplicates.

---

## Available options

1. ### **Upload a YouTube Short**
   The program looks for vertical videos in followed Instagram accounts. Steps:

   - It checks whether the video already exists in the database.
   - If the video is under 1 minute and meets the requirements, it shows a console link for user confirmation.
   - After confirmation, the video is uploaded automatically to **YouTube Shorts**.

   Tip: adjust the video name and description before uploading.

2. ### **Create video compilations**
   - Lets you select multiple videos to build a **compilation**.
   - You can choose how many videos to scrape from Instagram and whether to add an **intro/outro**.
   - This process is slower than Shorts because **MoviePy** is used for editing and formatting.

![AUTOYT](/PersonalWEB2.0/images/autpyt.png)

---

## Interested in the code?

{{< admonition info "Visit the project" >}}
[GitHub - Under maintenance]
{{< /admonition >}}
