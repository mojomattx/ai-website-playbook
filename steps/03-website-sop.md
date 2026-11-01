# Step 3: Write SOPs for every task

Step 3 of 34.

It comes after step 2, Build your project knowledge base, and before step 4, Write your brand style guide (coming soon).

## Why it matters

Every task on your site, like building a page or publishing a change, has one right way to do it.

Without written steps, that way lives in someone's head, and every page comes out a little different.

With them, you, your team and your AI do every task the same way, and every step gets checked so nothing is missed.

Write the steps once. Follow them every time.

## Rules

Each rule says how to do it and why it matters.

Its level says whether every site must follow it (Mandatory) or whether you get to pick if it's relevant for you (Recommended).

### Write an SOP for every template and recurring task, and follow it step by step

Level: Mandatory

**Every template and every recurring task has its own written SOP: read it before the work starts, and follow it step by step, in the written order.**

**How to do it:** An SOP is a process made of actions to take, like a checklist.

Before you work on a page built from a template, or on a task that comes back regularly, open its SOP.

Follow its steps in the written order, and skip or change a step only under the rule you choose below.

If there is no SOP yet, stop, write it, and get the owner's yes before you do the work (see the rule [Write every SOP in the same format](#write-every-sop-in-the-same-format)).

Recommended, your choice: decide who may skip or change a step.

If you check every step yourself, make it a rule that nobody skips, reorders or shortens a step without your yes.

Anyone who thinks a step looks wrong asks you before going further.

If you let your AI work on its own, you can let it decide, as long as it reports at the end of the task every step it skipped or did differently, and why.

**Why it matters:** Every page comes out the same way, so you don't fix the same errors again and again.

Skipped steps are where most rework comes from, so following every step saves you from doing the work twice.

### Write every SOP in the same format

Level: Recommended

**Write every SOP in the same format.**

**How to do it:** Use the same headings in every SOP, in this order.

Start with the purpose, when to use it, and the resources it needs.

Then say who does each step and with what tool.

Then list the build steps, the update steps, and the review points (where someone checks the work before it moves on).

End with the quality check, the common mistakes, and what makes the page go out of date and how costly that is.

Add a version number and a date at the top, and update both on every change.

**Why it matters:** Everyone finds what they need in any SOP right away, and nothing important gets left out.

### Write every SOP as a checklist, with a check for each step

Level: Mandatory

**Write every SOP as a checklist, and give each step a check you can see or test, never someone saying they did it.**

**How to do it:** Write each step as one line with a box in front of it, like "[ ] The page has a title".

Next to each step, write how to check it, like "open the page and look for its title".

When you can, pick a check a tool can run, like "the page returns a 200 status", the code a server sends back when a page loads fine.

Tick a box only after its check passes.

The task is finished only when every box is ticked.

To have a tool run the checks and tick the boxes for you, see the rule [Use a tool that marks each SOP step done](#use-a-tool-that-marks-each-sop-step-done).

**Why it matters:** You see right away what is finished and what is left, so nothing gets forgotten.

A check catches a step that wasn't really done, before it turns into a broken page later.

### Use a tool that marks each SOP step done

Level: Recommended

**Use a tool that marks each SOP step done only after its check passes, and blocks the next step until then.**

**How to do it:** Ask your AI to write a small script for your SOPs (a script is a small program that does a task for you).

The script keeps one record file per page or task, with one line per step and the date it was done.

After each step, it runs that step's check, like "the page loads" or "the page has a title", and writes the step's line only when the check passes.

For a step that needs a person's judgment, like choosing a headline, the check is the owner's yes: the script asks for it and writes who said yes.

It refuses to start the next step while the step before it has no line.

It stops with an error message when a step is done out of order or its check fails.

The page or task counts as finished only when every step has its line.

Never add a line by hand, and never let your AI add one just because it says the step is done.

**Why it matters:** AI tools and people sometimes say a step is done when it isn't, or skip one without noticing.

The tool catches a step that was skipped or not really done, before the next step builds on it, so you don't redo that work later.

### End every SOP, and every script, with a check

Level: Mandatory

**End every SOP, and every script, with a step that checks the result.**

**How to do it:** Make the last step a check of the finished result, like opening the live page or running the link check again.

If the check fails, fix the problem and check again.

**Why it matters:** The last check catches what earlier steps missed, before a visitor or a search engine sees it.

### A failed step stops the work

Level: Mandatory

**A failed step stops the work.**

**How to do it:** When a step fails, stop.

Fix the problem, then start again from that step.

Never skip it to continue with the next steps.

To have a tool stop the work for you, see the rule [Use a tool that marks each SOP step done](#use-a-tool-that-marks-each-sop-step-done).

**Why it matters:** Every step after a failure builds on something broken, so you would have to redo all of them.

### Report every step you skipped or changed

Level: Mandatory

**At the end of each task, report any step that was skipped or done differently, with the reason.**

**How to do it:** End every task report with a line like "Skipped: none", or "Step 3 skipped, with the owner's OK, because the page has no images".

If you work with an AI, ask it to add this line to every report.

**Why it matters:** A change nobody mentions is the hardest mistake to find later, and one line in the report saves you a long search.

### Turn repeat tasks that need no judgment into automatic systems

Level: Mandatory

**Turn every task that comes back regularly and needs no judgment into an automatic system, so it's cheap to run and makes no errors.**

**How to do it:** A task needs no judgment when the same input always gives the same result, like resizing images, updating page dates, or checking links (developers call this "deterministic").

List the tasks you do again and again.

Mark the ones that need no decision from a person.

Do the same inside each SOP: mark every step "automatic" or "judgment" (a judgment step needs someone to decide, like choosing a headline).

For each automatic task or step, have a script do it, or a scheduled job (a script that runs by itself at set times, like every night).

People and AI do only the judgment steps.

End each script with a check of its result, as the rule [End every SOP, and every script, with a check](#end-every-sop-and-every-script-with-a-check) says.

**Why it matters:** Once it's built, it's cheap to run and doesn't make errors, while people and AI tools make small mistakes on work they repeat.

### Turn your key rules into checks that block publishing

Level: Mandatory

**Turn the rules that matter most into automatic checks that stop publishing when a rule is broken.**

**How to do it:** Pick the rules that do the most damage when they're broken, like a broken link or a missing page title.

Ask your AI to write a script that checks them every time before you publish.

If a check fails, publishing stops until the problem is fixed.

**Why it matters:** A written rule can be skipped, but a blocking check can't, so the mistake never reaches your visitors.

### List every script and tool in one catalogue

Level: Mandatory

**List every script or tool you build in one catalogue, and always check it before you build a new one.**

**How to do it:** Create one page in the wiki called "Tools".

Add one line per tool: its name, what it does, and where it is saved.

Before you build a new tool, search this page first, so you never build the same thing twice.

**Why it matters:** You don't pay twice, in time or money, for a tool you already have.

### Brief anyone with the job and the rule pages to read

Level: Mandatory

**Brief anyone on a task by naming the job and the rule pages to read, and add only what they can't know.**

**How to do it:** A brief is the message that tells someone, a person or an AI, what to do.

Write the job in one line.

Link the wiki pages they must read.

Add only the facts specific to this task, like which page and by when.

Never paste a rule into the brief when it's already written in your wiki: link to it instead.

**Why it matters:** The brief stays short, and when a rule changes, every new brief already follows it, because it points to the wiki.

### Brief writers on what to cover, never a word count

Level: Recommended

**When you brief a writer, a person or an AI, tell them what the page must cover, never a word count to hit.**

**How to do it:** In the brief, list what the page must answer: every question the reader has, and the facts the page needs.

For example, write "answer how much it costs, how long it takes, and what's included" instead of "write 1,000 words".

When you review the text, check it against that list, not against a word count.

Check the page's length only after writing, as the rule "Give every page you want found in search at least 500 words of original content" in step 27 says.

**Why it matters:** A word count makes writers add filler content or cut true facts just to fit it, and both make the page worse.

A list of what to cover gives you a clear way to judge the text: every point is answered, or it isn't.

### Change only the lines that need it in shared files

Level: Mandatory

**When you change a file other people use, change only the lines that need it, and never rewrite the whole file.**

**How to do it:** This goes for a doc someone is reading or commenting on, a shared file, or a config (a settings file).

In a shared document, turn on suggestion mode or track changes, so the others see exactly what you changed.

Before you save a file, compare it with the old version, and check that only the lines you meant to change are different.

If you work with an AI, ask it to edit only those lines, never to rewrite the whole file.

**Why it matters:** Replacing the whole thing deletes other people's comments and changes without warning, and their work is lost.

### Stack your rules in layers

Level: Recommended

**Stack your rules in layers, from general to specific, and let the most specific layer win.**

**How to do it:** Order the layers like this: rules for every site, then for your type of site, your language, your tech stack (the tools your site is built and run with), your project, your voice, and each template.

When two layers say different things, follow the more specific one.

For example, your general rule says "keep every sentence short and casual", but your rule for the privacy policy says "include every item the law asks for: what you collect, why, how long you keep it, and who you share it with".

On the privacy policy, follow the privacy policy rule, or you would cut details the law asks for.

This matters once you run several sites, or several kinds of pages with their own rules.

With one simple site, you can skip it.

**Why it matters:** You write each rule once at the right level, and every project still gets its own exceptions without copying all the rules.

## Checklist

Run this checklist only when you audit a site that already exists.

Building a new site?

Don't run it yet.

Apply the rules above while you build, and the checks run at the pre-launch checklist step.

Check each line in your project's files or on the live site.

Mark a line yes only after that check, with who did it and the date.

Results are saved in your project's progress file, so nothing gets checked twice for no reason.

When you run the audit again, lines already marked yes are skipped, unless the files behind them changed since their verified date or the owner asks for a full re-check.

- [ ] 03-01 Every template and every recurring task has its own written SOP in the wiki | done by: n/a | verified: n/a
- [ ] 03-02 Every SOP uses the same headings in the same order, with a version number and a date at the top (Recommended) | done by: n/a | verified: n/a
- [ ] 03-03 Every SOP step is one line with a box, and has a written check you can see or test | done by: n/a | verified: n/a
- [ ] 03-04 Every page or task built from an SOP has a record file with one dated line per step (Recommended) | done by: n/a | verified: n/a
- [ ] 03-05 Every SOP and every script ends with a step that checks the finished result | done by: n/a | verified: n/a
- [ ] 03-06 The wiki says that a failed step stops the work, and that work starts again from that step once it is fixed | done by: n/a | verified: n/a
- [ ] 03-07 Every task report saved since the last audit ends with a line on the steps skipped or done differently, with the reason | done by: n/a | verified: n/a
- [ ] 03-08 Every SOP step is marked "automatic" or "judgment", and every automatic step is done by a script or a scheduled job | done by: n/a | verified: n/a
- [ ] 03-09 A script checks the key rules before every publish, and publishing stops when a check fails | done by: n/a | verified: n/a
- [ ] 03-10 The wiki has one "Tools" page that lists every script and tool, with its name, what it does, and where it is saved | done by: n/a | verified: n/a
- [ ] 03-11 Every brief saved in the project names the job in one line and links the wiki pages to read, with no rule pasted in | done by: n/a | verified: n/a
- [ ] 03-12 Every writer's brief saved in the project lists what the page must cover, and none sets a word count (Recommended) | done by: n/a | verified: n/a
- [ ] 03-13 No change to a shared file since the last audit replaced the whole file, as the version history shows | done by: n/a | verified: n/a
- [ ] 03-14 If the project uses rule layers, they are written down in order, from general to specific, with the most specific layer winning (Recommended) | done by: n/a | verified: n/a

## Next step

Next comes step 4, Write your brand style guide (coming soon).

In step 4, we'll show you how to write down everything there is to know about your brand, your voice, and the style rules that every page, and every piece of content, must follow, so it all looks and sounds like the same brand.

Every task now has its checklist, so nobody gets to say "I did it my way" anymore.
