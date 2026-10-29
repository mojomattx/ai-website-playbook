# How Any AI Uses This Repo

This file is for any AI model or AI tool pointed at this repo.

A person can read it too.

In this file, "the owner" is the person the website belongs to, or the person who decides for it.

## What this repo is

The AI Website Playbook by MojoSons Media.

It's a method to build a new website, or to audit and improve an existing one.

The method has 34 steps, one file each, in `steps/`. Steps not written yet are listed in `README.md` as coming soon.

Every written step has the same 4 parts: why it matters, mandatory rules, recommended practices, and a checklist of yes or no lines.

Step checklists are run only to audit an existing site; a new site applies the rules while it is built, and its checks run at the pre-launch checklist step (step 28).

## Read order

1. This file.
2. `README.md`: the list of 34 steps, with the written ones linked.
3. The one step the current task needs, in `steps/`.

Never load the whole repo at once.

Open any other file only when the current step points to it.

## Core rules

### 1. The owner approves first

Nothing is published, and nothing changes on the owner's live site, before the owner says yes.

Show what will change, then wait for a clear yes.

A yes covers that change only, never the next one.

### 2. One step at a time

Finish the current step before starting the next one.

On an existing site, fix one gap at a time, each with the owner's yes.

### 3. Yes only after a real check

Mark a checklist item yes only after checking it on the real site or the real files.

Never mark it yes from memory, or because it should be true.

Each line records who did the work and the date it was checked, in this format.

```
- [x] Every page has one H1 | done by: <person or AI tool> | verified: 2026-10-27
- [ ] Sitemap is never cached | done by: n/a | verified: n/a
```

These lines live in the owner's project, in a progress file in the owner's project.

When an item cannot be checked, leave it unchecked and tell the owner why.

The progress file keeps every audit result, so what was checked, by whom, and when is never lost.

When an audit runs again, never re-check a line for nothing:

- Skip lines already marked yes.
- Re-check a yes line only if the pages or files behind it changed since its verified date, or if the owner asks for a full re-check.
- Always check lines marked no or never checked.
- After each check, update the line's "done by" and "verified" date in the progress file.

### 4. Rules here, choices in the owner's setup file

The rules live in this repo.

The owner's choices (brand, voice, tools, and the rest) live in the owner's own setup file, in their project.

Never edit the rules in this repo to fit one project.

If a rule looks wrong for every website, tell the owner, who can suggest a change through `CONTRIBUTING.md`.

### 5. Ask when unsure

When this repo does not cover a situation, or a file it points to is missing, stop and ask the owner.

Never guess a rule.

## How to start

Ask the owner if the site is new or already live, and what it's about. Then start with step 1, or audit the written steps first if the site is live.
