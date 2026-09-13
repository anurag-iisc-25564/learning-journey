# learning-journey

📚 Anurag Anand's public learning log — a living feed of notes, repos, and discoveries.

🌐 **Live at:** https://anurag-iisc-25564.github.io/learning-journey/

Built with **Jekyll** + GitHub Pages. Posts appear **newest first**.

---

## ➕ Adding a new post

Create a file in `_posts/` with this naming convention:

```
_posts/YYYY-MM-DD-title-with-dashes.md
```

### Minimal template

```markdown
---
layout: post
title: "What I Learned About XYZ"
date: 2026-09-14
description: "One-line summary shown in the feed."
tags: [tag1, tag2]
---

Your content in Markdown here...
```

### With a GitHub repo link

```markdown
---
layout: post
title: "Built a Mini Transformer from Scratch"
date: 2026-09-15
description: "Implemented attention, positional encoding, and training loop."
tags: [deep-learning, nlp, pytorch]
repo: https://github.com/anurag-iisc-25564/mini-transformer
---

Notes here...
```

---

## Available front-matter fields

| Field         | Required | Description                                      |
|---------------|----------|--------------------------------------------------|
| `layout`      | ✅       | Always `post`                                    |
| `title`       | ✅       | Title shown on card and post page                |
| `date`        | ✅       | `YYYY-MM-DD` — determines sort order            |
| `description` | optional | Short blurb shown in the feed card               |
| `tags`        | optional | List of topic tags                               |
| `repo`        | optional | GitHub repo URL — shows a button on the post     |

---

## File structure

```
├── _config.yml
├── index.html          ← feed (auto-updates)
├── _layouts/
│   ├── default.html
│   └── post.html
├── _posts/
│   ├── 2026-09-13-welcome.md   ← example post
│   └── ...                     ← add yours here
├── assets/
│   └── css/style.css
└── README.md
```

## Deploy

1. Create a **new** repo named `learning-journey`
2. Push all files to `main`
3. Go to **Settings → Pages → Source: main branch / root**
4. Site goes live at `https://anurag-iisc-25564.github.io/learning-journey/`
