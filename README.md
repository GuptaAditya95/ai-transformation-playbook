# AI Transformation Playbook

Lessons and frameworks from my AI transformation leadership course, published at
https://guptaaditya95.github.io/ai-transformation-playbook/

## Workflow for each lesson

Each lesson moves through three folders, matching three stages:

| Stage | Folder | Published? |
|---|---|---|
| 1. Pointers: raw notes right after the lesson | `notes/` | No (excluded from the site) |
| 2. Framework: shaping the notes into a lesson | `_drafts/` | No (Jekyll skips drafts) |
| 3. Page: the finished lesson | `_posts/` | Yes, and subscribers are notified |

1. Copy `templates/notes.md` to `notes/2026-11-02-topic.md` and dump your pointers.
2. Copy `templates/lesson.md` to `_drafts/topic.md` and distil the notes into the framework.
3. When it's ready, move it to `_posts/2026-11-02-topic.md` (the date prefix is required) and push.
   The site rebuilds in about a minute, the RSS feed updates, and email subscribers get it.

Note: the repo is public, so `notes/` and `_drafts/` are visible on GitHub even though
they don't appear on the site. Keep anything private out of them.

## Subscriptions

- **RSS** is automatic at `/feed.xml`.
- **Email**: create a free feed at https://follow.it using the RSS URL above, then paste the
  form's action URL into `subscribe.email_form_action` in `_config.yml`. Until then only RSS
  and GitHub Watch are shown.

## Preview locally (optional)

```
bundle install
bundle exec jekyll serve --drafts
```
