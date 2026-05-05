# Contributing — Lo-Rig website

Thanks for contributing! This guide explains how to add and format project updates so they appear correctly on the website.

---

## Repository structure (short)

* `mkdocs.yml` — site configuration
* `docs/` — all website content

  * `docs/updates/posts/` — project update posts (one `.md` file per post)
  * `docs/assets/images/updates/` — images for posts
* `stylesheets/extra.css` — additional styling
* `overrides/` — theme customisation

---

## Creating a new update post

1. Create a new Markdown file in:

   ```
   docs/updates/posts/
   ```

2. Name the file using the format:

   ```
   YYYYMMDD-short_title.md
   ```

   Example:

   ```
   20260505-bhutan_fieldwork.md
   ```

3. The `slug` in the front matter **must match the file name**:

   ```
   slug: 20260505-bhutan_fieldwork
   ```

---

## Post format (copy–paste template)

Use the following template:

```
---
title: Example Title
date: 2026-05-05
categories:
  - Project Development
tags:
  - Monkha
  - Fieldwork
authors:
  - your_name
slug: 20260505-example
image: assets/images/updates/20260505-example/image.png
---

# Example Title

**05 May 2026**

Short introductory paragraph.

<figure markdown>
![Caption](/assets/images/updates/20260505-example/image.png){ width="85%" }
<figcaption>
Caption text.
</figcaption>
</figure>
```

---

## Images

* Store images in:

  ```
  docs/assets/images/updates/YYYYMMDD-post_name/
  ```

* Reference them like this:

  ```
  ![](/assets/images/updates/YYYYMMDD-post_name/image.png)
  ```

* Use clear, descriptive filenames.

---

## Terminology (important)

Please use the following consistently:

* **Monpa** — people / community
* **Monkha** — language

---

## Golden rules

* Keep posts concise (usually 1–3 paragraphs is enough)
* Use clear, neutral language (avoid informal tone)
* Check spelling of names and places carefully
* Keep formatting consistent with existing posts

---

## Before submitting

* Ensure `title`, `date`, and `slug` are included
* Confirm the slug matches the filename
* Check that images load correctly
* Preview locally if possible

---

## Local preview (optional)

To preview the site locally:

```bash
pip install -r requirements.txt
mkdocs serve
```

Open:

```
http://127.0.0.1:8000
```

---

## If you are not familiar with Git

You can still contribute:

* Send your text and images to a project member
* Or share a draft (Word / Google Docs)

We will format and upload it for you.

---

## Questions

If you're unsure about anything, feel free to ask a core project member or open an issue.
