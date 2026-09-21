# Contributing

This repo is a curated list of open-source projects built with Jev, TypeSafe AI's System One Model. Contributions are welcome, but every entry goes through a quick review to keep the collection tight and non-redundant.

## Before you start

Open an issue or a draft PR naming the project before writing up the entry. Check the table of contents in `README.md` first to see if something similar already exists.

## What qualifies

A project can be added if it meets **all** of these:

- It's hosted on GitHub and has **50 or more stars**, with visible signs of real usage (issues, forks, recent commits) — not a fresh repo with inflated or vanity stars.
- It actually calls or implements the Jev decision interface (a typed question in, a `Choice`/`Score`/boolean out) — not just a passing mention of TypeSafe AI or Jev in a README.
- It's still functional — check it against the current Jev API or a recent release before submitting.

Star count is a filter, not a quality guarantee. A [review of 287 open-source Jev projects](https://www.reddit.com/r/LLMDevs/comments/1wko2e5/i_reviewed_287_opensource_jev_projects_here_are/) found most repos either misuse Jev or barely touch it — verify the project genuinely uses typed decisions before submitting it.

## One entry per repo, not per feature

Each entry represents a repository or publisher, not an individual demo or script inside it.

## Where an entry goes

Entries are grouped into categories in `README.md` (Coding Agents & Dev Tooling, Browser & Computer-Use Automation, Search Retrieval & Data Labeling, SDKs & Platform Integrations, Open-Source Jev Alternatives, Applied Decisions). Add a new category only if an entry doesn't fit any existing one, and keep the total category count small.

Within a category, entries are sorted alphabetically by repo/publisher name.

Add a matching entry to the table of contents at the top of `README.md`, linking to the category's heading anchor.

## Writing an entry

Format:

```
- **[repo-name](link-to-repo)** — one sentence on what the project does and how it uses Jev.
```

- Description is factual and third person — no marketing language, and written in your own words rather than copied from the repo's README.
- Link to the repository root.

## Style

Writing must be simple, concise, and factual — no buzzwords, no unverified claims about what a project does.

## Submitting

Open a PR adding the entry. Mention the current star count and how the project uses Jev so it can be reviewed.
