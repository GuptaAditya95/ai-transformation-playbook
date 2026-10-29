# AI Transformation Playbook

**Practical frameworks for leading AI transformation, written up one lesson at a time.**

👉 **Read it here: https://guptaaditya95.github.io/ai-transformation-playbook/**

I'm Aditya, and I'm working through a course on leading AI transformation. After each lesson I turn my
notes into a framework you can reuse, show it working on a realistic case study, and publish it on the
site above. It's written for business leaders, so no technical background is needed.

## Lessons

| # | Lesson | Framework | What it helps you do |
|---|---|---|---|
| 1 | [Build your AI leadership strategy](https://guptaaditya95.github.io/ai-transformation-playbook/lessons/build-your-ai-leadership-strategy/) | The Translation Method | Turn business goals into 2–3 measurable AI bets |
| 2 | [AI literacy for business leaders](https://guptaaditya95.github.io/ai-transformation-playbook/lessons/ai-literacy-for-business-leaders/) | AI Readiness and Responsible AI | Check if you can scale AI, and build it responsibly |

Every lesson follows the same shape: **key pointers → the framework → a case study → putting it to work.**
The case studies follow Meridian Insurance, a fictional company, so you can see the frameworks build on each other.

## Follow along

- **Email or RSS:** see the [Subscribe page](https://guptaaditya95.github.io/ai-transformation-playbook/subscribe/)
  or add [the RSS feed](https://guptaaditya95.github.io/ai-transformation-playbook/feed.xml) to your reader.
- **GitHub:** click **Watch** at the top of this page.

Spotted a mistake or have a better example? [Open an issue](https://github.com/GuptaAditya95/ai-transformation-playbook/issues).

## What's in this repository

| Folder | What it is |
|---|---|
| `_posts/` | The published lessons (this is what you see on the site) |
| `notes/` | My raw notes from each lesson, before they become a framework |
| `_drafts/` | Lessons in progress, not yet on the site |
| `templates/` | The templates I use for notes and lessons |
| everything else | The site itself, built with Jekyll and hosted on GitHub Pages |

<details>
<summary><strong>How I publish a lesson</strong> (for me, or anyone reusing this setup)</summary>

1. Copy `templates/notes.md` to `notes/YYYY-MM-DD-topic.md` and write down the raw pointers.
2. Copy `templates/lesson.md` to `_drafts/topic.md` and distil the notes into a framework and case study.
3. When it's ready, move it to `_posts/YYYY-MM-DD-topic.md` and push. The site rebuilds in about a minute,
   and the RSS feed and email subscribers pick it up.

**Email subscriptions:** create a free feed at https://follow.it using the RSS URL, then paste the form's
action URL into `subscribe.email_form_action` in `_config.yml`.

**Preview locally:** `bundle install && bundle exec jekyll serve --drafts`
</details>
