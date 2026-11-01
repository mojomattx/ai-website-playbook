# Step 2: Build your project knowledge base

Step 2 of 34.

It comes after step 1, Write your website project plan, and before step 3, Write SOPs for every task (coming soon).

## Why it matters

A project knowledge base is the set of written pages that hold everything about your website project: its facts, rules, decisions, and how the site runs.

Without it, every answer depends on someone's memory or an old chat.

With it, you, your team and your AI tools work from the same facts, and nobody starts from zero.

Write it down once. Never explain it twice.

## Rules

Each rule says how to do it and why it matters.

Its level says whether every site must follow it (Mandatory) or whether you get to pick if it's relevant for you (Recommended).

### Keep one project wiki in your repository

Level: Mandatory

**Keep one project wiki (the pages that explain how your project works) as plain text files in a single folder at the top level of the site's repository (the folder that holds all the site's files and their history).**

**How to do it:** Create one folder for the wiki at the top level of the repository, for example `wiki`.

Write each page as a plain text file in Markdown, a simple text format any person or AI tool can read.

Make sure the wiki is never uploaded to the live site: open yoursite.com/wiki in a browser, and it must show "not found".

Never put it inside a folder that belongs to one AI tool.

**Why it matters:** Everyone, people and AI tools, reads the same rules, so nobody works from an old copy.

When you change people or tools, the wiki stays with the site's files, so nothing is lost.

### Cover the basics in your wiki from day one

Level: Mandatory

**The wiki covers a minimum set of topics from the start.**

**How to do it:** Create one page for each of these: an overview of the project, the brand style guide, the content guidelines, design, images, author bios, and social media accounts.

Your SOPs (an SOP is a process made of actions to take, like a checklist) and a reading order for the wiki come on top of these: the SOPs are covered in the next step, and the reading order further down this step.

Write the few facts you already know on each page, and add the rest as you go.

**Why it matters:** The basics are written down from day one, so nobody loses time asking for them or guessing them.

### Give the project a "start here" page

Level: Mandatory

**Give the project a map, a "start here" reading order, and a starting point for each role.**

**How to do it:** On the first page of the wiki, list each folder and what it holds.

Then write the order to read the wiki pages in.

Then say where a writer, a developer, an AI tool, or a manager should start.

**Why it matters:** Someone new can start working on day one instead of searching for things, which saves you time explaining.

### Write plain instructions anyone can follow

Level: Mandatory

**Write every wiki page, SOP, and tool as plain instructions that any person or any AI tool can follow.**

**How to do it:** For each SOP, write what to do, in what order, and how to check it worked.

Never write it as a message to one AI tool, like "please do this for me".

Anything that only works with one tool goes in its own section, with a clear title, and never contradicts the shared rules.

**Why it matters:** You can switch tools or AI models without rewriting your wiki.

A new person can follow the same wiki on day one, without learning your tools first.

### Keep each fact and rule in one place

Level: Mandatory

**Keep each fact and each rule in one place, and link to it everywhere else.**

**How to do it:** When you need a rule in a second place, add a link to it instead of copying the text.

When you find the same rule written twice, keep the best version and replace the other with a link.

**Why it matters:** When a rule changes, you update one page, not five.

Copies stop matching over time, and then people follow the old version by mistake.

### Keep your key facts in data files

Level: Mandatory

**Keep the project's key facts (figures, prices, dates, names, company details) in data files that every page reads from, each fact in one place only.**

**How to do it:** A data file is a simple file that lists facts the site's pages can read, like `data/prices.json` for your prices.

Write each fact there once.

Have every page that shows the fact read it from that file, instead of typing it into the page.

Keep your company details in their own file, like `COMPANY.md`: legal name, address, contact details, the area you serve, the brand name, where the logo file is saved, and the links to your social media accounts.

The header, the footer, the legal pages and the schema (code that tells search engines who you are) read them from that file, so when a social link or the logo changes, you change one line, not every page.

When you need a fact the file doesn't hold yet, add it to the file first, never write it from memory.

When a company detail is missing, ask the owner and save the answer, never invent one.

**Why it matters:** When a price changes, you update it once and every page shows the new price.

A fact typed by hand on ten pages gives you ten chances to make a mistake, and a wrong price or date on your page costs you trust.

### Keep one shared instructions file for your AI tools

Level: Mandatory

**Keep the instructions for AI tools in one shared file, and have each tool's own setup file point to it.**

**How to do it:** Write the project's instructions for AI tools once, in one shared file, for example `AGENTS.md`.

Some AI tools only read their own [setup file](01-website-project-plan.md#write-one-short-setup-file), under their own name.

For those, create that setup file with one line that tells the tool to read the shared file.

**Why it matters:** Every AI tool follows the same rules, and when a rule changes, you update it in one place.

### Share writing rules across languages

Level: Recommended

**If your site is in several languages, keep the writing rules they share in one file, and give each language its own file for what only applies to it.**

**How to do it:** Write each writing rule once, in the shared file.

Then give each language its own file, with examples and the rules that only apply to that language.

**Why it matters:** You update a rule once for every language, instead of fixing it in each language file one by one.

### Keep a technical handover page

Level: Mandatory

**Keep a technical handover page that lists every service the site uses and how the site runs.**

**How to do it:** List every service the site uses, and for each one, write where you manage it (the website you log in to) and the account ID.

The registrar: the company you bought the domain from.

The DNS: the settings that connect your domain to your hosting and your email, for both example.com and www.example.com.

The hosting: the service that keeps your site online, and where the site's files get uploaded when you publish.

The code host: the online service that stores your site's files and their history, if you use one.

The database, payments, email, and analytics (the tool that counts your visitors), if you use them.

Then add the email DNS records.

Add the redirects (rules that send visitors from an old address to a new one).

Add the endpoints (the addresses your site's code calls to send or fetch data).

Add the data you store about visitors.

Add an emergency plan: what to do, step by step, when the site goes down.

Add a "How we publish" section: every step that takes a finished change to the live site, in order (publishing a change is also called deploying).

End that section with what to do after publishing, like clearing the cache (the stored copy of your pages that the host shows visitors) and checking the live page.

Read this page before you ask anyone a technical question.

**Why it matters:** When the site goes down, you find the right login and the right steps right away, instead of searching through old emails.

When someone new takes over, they don't depend on one person's memory, so you can change developers without losing anything.

Nobody has to work out how to publish again, and no step gets forgotten, so publishing doesn't break the site.

### Keep one state file

Level: Mandatory

**Keep one state file with the project's decisions, facts, and paused items, separate from the to-do list.**

**How to do it:** Create one file, for example `STATE.md`, with three lists: decisions, facts about the project, and items paused for later.

For each decision, add one dated entry: what was decided, why, who decided it, and which older decision it replaces, if any.

Never delete or change an old decision: add a new entry instead.

When a decision changes a rule, update that rule's wiki page too.

Update the file every time one of these changes.

Keep your to-do list somewhere else, so this file only shows where the project stands, not what's left to do.

**Why it matters:** Anyone can pick up the project after a break without asking what happened last time, so no time is lost catching up.

Months later, you can see why something was done, so nobody wastes time reopening a question that was already decided.

### Use short and factual wiki pages

Level: Recommended

**Keep wiki and rule pages short and factual.**

**How to do it:** For each rule, write the rule and a short reason.

Add a date next to any fact that can go out of date.

Leave the history out of the page, since version control (the system that saves every version of your files) and the state file already keep it.

**Why it matters:** People read short pages to the end and skip parts of long ones.

The shorter a rule is, the more it gets followed.

### Write down what you said no to

Level: Recommended

**Write down every suggestion, tool or feature you chose not to use, with the reason.**

**How to do it:** Create one page called "Not adopted" in your wiki, separate from your state file, so the state file stays short.

Add one line each: what was suggested, by whom or where, and why you said no.

For a tool or feature you left out of your setup, write what it is and why.

**Why it matters:** The same suggestion doesn't come back every few months, so you don't spend time discussing it again.

### Write every rule and decision in the wiki the same day

Level: Mandatory

**Write every rule and decision in the wiki the same day it is made.**

**How to do it:** At the end of any discussion that sets a rule, add it to the right wiki page before you move on to the next task.

If you work with an AI, ask it to add the rule to the wiki at the end of the session.

A rule that lives only in a chat, a commit message (the short note saved with each change to the site's files), or a code comment doesn't count.

**Why it matters:** Rules that aren't written down get forgotten, and then you spend time fixing the same mistake again.

### Update the wiki with the change

Level: Mandatory

**Update the wiki page that describes a change at the same time as the change, in the same commit.**

**How to do it:** When you change something on the site, find the wiki page that describes it and update it.

Save both changes together, as one commit.

If an AI makes the change, ask it to update the wiki page in the same step.

**Why it matters:** The next person, or your AI, reads a wiki page that matches the site, so they don't build on wrong information.

### Fix the wiki or the site the same day they disagree

Level: Mandatory

**When the wiki disagrees with the site or with someone's memory, fix whichever is wrong the same day.**

**How to do it:** Check which one is right: the wiki, the live site, or what the person remembers.

Fix the one that's wrong, then tell the owner what was wrong and what you changed.

Until it's fixed, follow the wiki.

**Why it matters:** Everyone follows the same version while it's being fixed, so nobody builds on a guess.

Fixing it the same day stops the mistake from spreading to new pages.

### Cite only sources from your approved list

Level: Recommended

**Keep a list of approved sources for each project, and cite only those.**

**How to do it:** Write the list in the setup file.

For example, a statistics site might list the official organization for its topic and one or two major news outlets.

Before you publish a fact, check that it comes from a source on the list.

If it doesn't, find it on a listed source, or leave it out.

**Why it matters:** A random blog or a search summary can be wrong, and a wrong fact on your page costs you trust.

### Log your research and audits

Level: Recommended

**Keep your research and audits in one log, and say where each finding comes from and how sure it is.**

**How to do it:** Create one page in the wiki called "Research and audits".

Add every piece of research or audit (a full check of your site) there, like keyword research, competitor checks, speed tests or a site audit.

For each one, write what was checked, the date, and its limits, like "checked in the US only".

Next to each finding (a number, a fact or a test result), name the source and how sure it is, like "measured on the live site" or "read in one blog post".

Write "not measured" when it wasn't measured.

**Why it matters:** You don't spend time or money redoing research you already have, and you know how old it is before you trust it.

You don't build on a guess written like a fact, so you don't redo the work when the guess turns out wrong.

### List every promotion on the site

Level: Recommended

**Keep one page listing every marketing feature and promotional block on the site: current, planned, and ended.**

**How to do it:** A promotional block is any box, banner or button on the site that promotes something, like a product, a newsletter or a special offer.

Create one page with three sections: current, planned, and ended.

Add one line per item, with where it shows, what it links to, and a "last checked" date.

When an item ends, move its line to "ended" instead of deleting it.

**Why it matters:** Old promotions don't stay live by mistake, showing visitors something that no longer exists, and you can see what ran before.

### Share one known-issues log across your sites

Level: Recommended

**If you run several sites of the same kind, keep one known-issues log that they all share.**

**How to do it:** Create one page that all those sites can read.

A known issue is a problem you hit once and fixed, like a form that stopped sending emails.

For each issue, write what went wrong, which site it happened on, and the fix.

Read this page before you build a new site.

**Why it matters:** The next site starts with the fix already known, so you don't lose time on the same problem twice.

### Let your AI fill in the progress file

Level: Mandatory

**Keep a progress file with the playbook's checklist, filled in by your AI during each audit.**

**How to do it:** Create one file, for example `PROGRESS.md`, with one line per task or check, each with a box.

Your AI ticks each box during an audit of your site, and writes the date it checked, so you never update this file by hand.

A box is ticked only after the result has been checked.

Next time, the AI skips what already passed, unless the page changed since.

**Why it matters:** Anyone, you or your AI, can see what is done and what is left without asking, and a ticked box can be trusted.

## Checklist

Run this checklist only when you audit a site that already exists.

Building a new site?

Don't run it yet.

Apply the rules above while you build, and the checks run at the pre-launch checklist step.

Check each line in your project's files or on the live site.

Mark a line yes only after that check, with who did it and the date.

Results are saved in your project's progress file, so nothing gets checked twice for no reason.

When you run the audit again, lines already marked yes are skipped, unless the files behind them changed since their verified date or the owner asks for a full re-check.

- [ ] 02-01 The wiki is one folder of plain text files at the top level of the repository, not inside a folder that belongs to one AI tool | done by: n/a | verified: n/a
- [ ] 02-02 The wiki folder's address on the live site (for example yoursite.com/wiki) shows "not found" | done by: n/a | verified: n/a
- [ ] 02-03 The wiki has a page for the overview, the brand style guide, the content guidelines, design, images, author bios, and social media accounts | done by: n/a | verified: n/a
- [ ] 02-04 The first wiki page lists each folder, the reading order, and where each role starts | done by: n/a | verified: n/a
- [ ] 02-05 Every SOP says what to do, in what order, and how to check it, without being written as a message to one AI tool | done by: n/a | verified: n/a
- [ ] 02-06 No rule is written out in full in two places | done by: n/a | verified: n/a
- [ ] 02-07 Every fact shown on more than one page (a price, a date, a name) is read from a data file, not typed into the page | done by: n/a | verified: n/a
- [ ] 02-08 The company details live in their own file, and the footer, the legal pages and the schema read them from it | done by: n/a | verified: n/a
- [ ] 02-09 The instructions for AI tools are in one shared file, and each tool's own setup file only points to it | done by: n/a | verified: n/a
- [ ] 02-10 If the site is in several languages, the writing rules they share are in one file, and each language has its own file with only the rules and examples for that language (Recommended) | done by: n/a | verified: n/a
- [ ] 02-11 The technical handover page lists every service with where it's managed and its account ID, plus the email DNS records, the redirects, the endpoints, the data stored, an emergency plan, and every step to publish a change, with the checks after publishing | done by: n/a | verified: n/a
- [ ] 02-12 One state file holds dated decisions, facts, and paused items, and no to-do items | done by: n/a | verified: n/a
- [ ] 02-13 On the wiki pages, each rule is written as the rule plus a short reason, each fact that can change (like a price) has the date it was checked next to it, and no page lists its own past versions or old changes (Recommended) | done by: n/a | verified: n/a
- [ ] 02-14 The wiki has a "Not adopted" page, separate from the state file, with what was suggested, by whom or where, and why it was not implemented (Recommended) | done by: n/a | verified: n/a
- [ ] 02-15 Every rule the team follows is written on a wiki page | done by: n/a | verified: n/a
- [ ] 02-16 Every change since the last audit was saved in the same commit as the update to its wiki page | done by: n/a | verified: n/a
- [ ] 02-17 The technical handover page and the company details file match what is live (services, address, contact details) | done by: n/a | verified: n/a
- [ ] 02-18 The setup file has a list of approved sources, and it includes the only sources the content can cite: every source cited on the site is on that list (Recommended) | done by: n/a | verified: n/a
- [ ] 02-19 The wiki has a "Research and audits" page, with the date and limits of each research or audit, and next to each piece of information it found, its source and how sure that information is (Recommended) | done by: n/a | verified: n/a
- [ ] 02-20 One page lists every block or element used for promotions or marketing, under current, planned, and ended, each with where it shows, its link and a "last checked" date, and every one live on the site is under current (Recommended) | done by: n/a | verified: n/a
- [ ] 02-21 If the project is one of several sites of the same kind, they share one known-issues page, with what went wrong, on which site, and the fix (Recommended) | done by: n/a | verified: n/a
- [ ] 02-22 The progress file exists, and every ticked box has a date | done by: n/a | verified: n/a

## Next step

Next comes step 3, Write SOPs for every task (coming soon).

In step 3, you write the step-by-step SOP for every task on your site, so every page gets built the same way, the right way.

Your project now remembers more than you do, and now it will (hopefully) never say "I thought you knew".
