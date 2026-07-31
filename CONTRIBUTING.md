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
  - Fieldwork and Communities
tags:
  - Monkha
  - Field Visit
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

## Categories and tags

Use **one category per post**. Categories should stay broad so that the update archive remains easy to browse. Use tags for more specific topics, places, languages, institutions, tools, and activity types.

### Standard categories

Choose one of the following categories:

* **Project News** — project milestones, team updates, administrative updates, institutional home, project setup
* **Fieldwork and Communities** — field visits, community meetings, community-facing updates, local conditions affecting fieldwork
* **Training and Capacity Building** — training sessions, workshops, summer schools, teaching activities, capacity-building events
* **Outreach and Dissemination** — talks, seminars, conference presentations, media coverage, public-facing visibility
* **Partnerships and Networks** — institutional visits, collaborations, research networks, external academic relationship-building

Do not create new categories unless there is a clear need and the website maintainer agrees.

### Recommended tag usage

Tags should be specific and reusable. They can include:

* Languages and communities, for example: `Gongduk`, `Gongdue Kha`, `Monpa`, `Monkha`
* Places, for example: `Bhutan`, `Riti`, `Chungseng`, `Phuzur`, `Jangbi`, `Wangling`, `Trongsa`, `Thimphu`
* Institutions, for example: `Trinity College Dublin`, `Trinity Long Room Hub`, `Centre for Bhutan and GNH Studies`, `IIT Guwahati`, `Tezpur University`, `Rajiv Gandhi University`
* Activity types, for example: `Field Visit`, `Community Engagement`, `Workshop`, `Summer School`, `Class`, `Talk`, `Research Seminar`, `Conference`, `Conference Presentation`, `Media`, `Collaboration`, `Institutional Collaboration`
* Research themes and tools, for example: `Language Documentation`, `Linguistic Fieldwork`, `Historical Linguistics`, `Trans-Himalayan Languages`, `Speech Technology`, `ASR`, `Forced Alignment`, `ELAN`, `FLEx`, `Human Language Technology`, `Human-Centred Technology`
* Project roles or administration, for example: `Team`, `Research Assistants`, `PhD Student`, `Postdoctoral Researcher`, `Administration`, `ERC`

Keep tags consistent with existing posts. For example, use `Field Visit` rather than alternating between `Field Visit` and `Fieldwork` when referring to a specific project visit.

---

## Choosing the right category

Use this quick guide when classifying a post:

| If the post is mainly about... | Use this category | Put these details in tags |
| --- | --- | --- |
| A project start, team member, institutional home, or internal milestone | `Project News` | `Team`, `PhD Student`, `Postdoctoral Researcher`, `ERC`, `Trinity College Dublin` |
| A village visit, field recording trip, community meeting, or fieldwork access issue | `Fieldwork and Communities` | `Field Visit`, `Community Engagement`, village names, language names, `Media`, `Infrastructure` |
| A workshop, training session, summer school, or teaching activity | `Training and Capacity Building` | `Workshop`, `Summer School`, `Class`, `Research Assistants`, `ASR`, `Linguistic Fieldwork` |
| A talk, research seminar, conference presentation, or media mention | `Outreach and Dissemination` | `Talk`, `Research Seminar`, `Conference`, `Conference Presentation`, `Media`, topic tags |
| A university visit, external collaboration, or research network meeting | `Partnerships and Networks` | `Collaboration`, `Institutional Collaboration`, institution names, country or region tags |

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
* Use one standard category per post
* Use tags for specific languages, places, institutions, tools, and activity types
* Check spelling of names and places carefully
* Keep formatting consistent with existing posts

---

## Before submitting

* Ensure `title`, `date`, and `slug` are included
* Confirm the slug matches the filename
* Use one of the standard categories listed above
* Check that tags are spelled consistently with existing posts
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
