# hanna-makes-robots

Build log for my robotics learning journey.
Site: [hannakesrobots.github.io](https://github.com)

---

## How to add a new post

Open `posts.json` and add a new object at the **top** of the array (newest first):

```json
{
  "date": "Apr 5, 2026",
  "week": "Week 2",
  "tag": "phase1",
  "tagLabel": "Phase 1",
  "title": "Your entry title here",
  "body": [
    "First paragraph. Use <strong>bold</strong> for emphasis.",
    "Second paragraph. Each string in this array becomes a paragraph.",
    "Third paragraph if needed."
  ],
  "links": [
    { "label": "Link text", "url": "https://example.com" }
  ]
}
```

Remove the `"links"` field entirely if you have no links for that entry.

---

## Tag options

| tag value | colour | use for |
|-----------|--------|---------|
| `day0`    | orange | milestone / start |
| `phase1`  | yellow | Phase 1 learning |
| `win`     | green  | something worked |
| `fail`    | red    | something broke |

Add new tag styles in `index.html` under `.entry-tag.yourname` if needed.

---

## File structure

```
/
├── index.html     ← site layout and styles (rarely edited)
├── posts.json     ← all build log entries (edit this to add posts)
└── README.md      ← this file
```

---

## Deploy to GitHub Pages

1. Push both files to a GitHub repo
2. Settings → Pages → Source: main branch / root
3. Live at `yourusername.github.io/repo-name`
