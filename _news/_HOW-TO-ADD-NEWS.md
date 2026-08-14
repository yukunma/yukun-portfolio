# How to add a news item （怎么加一条 news）

**No coding needed.** One news item = one file in this `_news/` folder.

## 3 steps

1. Copy `_TEMPLATE.md` (in this folder) to a new file.
2. Name it `YYYY-MM-DD-short-title.md`, e.g. `2026-09-15-nber-talk.md`.
   (The file name is only for your own convenience — what actually shows up
   on the site is the `date:` line inside the file.)
3. Edit the `date:` line and the text at the bottom. Save. Done.

Files starting with `_` (like this one and the template) are ignored by the
site, so they never show up as news.

## The file format

```
---
layout: post
date: 2026-09-15 09:00:00-0400
inline: true
related_posts: false
---

Invited talk at the NBER Summer Institute.
```

(shows up as: **Sep 2026** — Invited talk at the NBER Summer Institute.)

Only two things to change:
- `date:` — keep the `-0400` at the end. Only the **month and year** are shown
  on the site ("Sep 2026"), but you still have to write a full date here — the
  day is what puts items in the right order inside the same month. If you don't
  care, just use the 1st. Newest items automatically appear on top.
- The text after the `---` — one or two sentences.

## House style: no verbs, no tense

Write each item as a **headline, not a sentence** — the date on the left
already says when it happened, so the text should not say "will" or "gave".

| Write this                    | Not this                             |
| ----------------------------- | ------------------------------------ |
| Invited talk at UC Davis.     | ~~Will give a talk at UC Davis.~~    |
| Invited talk at CUHK.         | ~~Gave a talk at CUHK.~~             |
| Paper accepted at *JoE*.      | ~~My paper was accepted at *JoE*.~~  |
| Joined the University of ...  | ~~I have joined the University ...~~ |

**Why this matters:** an upcoming talk and a past talk then look identical, so
you never have to go back and rewrite "will give" into "gave" after the event.
Mixing the two tenses in one list is what looks unpolished.

Useful openers: `Invited talk at ...`, `Seminar at ...`, `Presentation at ...`,
`Paper accepted at ...`, `New working paper: "..."`, `Visiting ...`.

## Text tricks (Markdown)

| What you want            | What you type                              |
| ------------------------ | ------------------------------------------ |
| **bold**                 | `**bold**`                                 |
| *italic* (journal names) | `*Journal of Econometrics*`                |
| a link                   | `[[slides]](https://example.com/deck.pdf)` |
| an emoji                 | `:tada:`                                   |

Keep it to one paragraph — inline news items are single-line by design.

## Upcoming talks (future dates)

A future date is fine — it shows up right away, pinned at the top of the list.
Because of the no-tense rule above, an upcoming talk is written exactly like a
past one ("Invited talk at UC Davis."), so there is nothing to edit once the
date passes. Just leave it alone.

## Longer posts (optional)

If a news item deserves a full page (photos, long text), set `inline: false`
and add a `title:` line. The homepage will then show the title as a clickable
link to its own page:

```
---
layout: post
title: Trip report — Midwest Econometrics Group 2026
date: 2026-10-10 09:00:00-0400
inline: false
related_posts: false
---

Long text goes here, as many paragraphs as you like.
```

## Settings you may want to touch (in `_config.yml`)

- `news_limit: 5` — how many items show on the homepage. The `/news/` page
  always shows all of them.
- `news_scrollable: true` — the homepage list scrolls instead of growing.
- `future: true` — keep this on, or future-dated items (upcoming talks) lose
  their own page.

## Preview locally

```
bundle exec jekyll serve
```
then open http://localhost:4000 — the news section is on the homepage.
