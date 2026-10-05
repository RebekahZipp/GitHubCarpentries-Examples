# TRY prompts

Use these prompts after cloning the example.

## 1. Locate

```bash
pwd
git rev-parse --show-toplevel
```

**TALK:** What is the difference between those two answers?

## 2. Observe

```bash
git status
git log --oneline
git remote -v
```

**TALK:** What does each command tell us that the others do not?

## 3. Investigate the files

Read the README, data, notes, ignore rules, license, and citation file.

**TALK:** Add one observation to Teams or say it aloud.

## 4. Test an ignore rule locally

Create a harmless PNG-named placeholder or use an instructor-provided generated file, then inspect:

```bash
git status
git status --ignored
git check-ignore -v PATH
```

**TALK:** What evidence tells you why Git is ignoring the path?

## 5. Transfer

Before making substantive changes, move to your **BUILD repository**.

Finish this sentence:

> "The example repository helped me inspect ___. My own repository is where I will build ___."


## Workshop continuity: guacamole carries forward

This TRY repository now includes `guacamole.md` so the Oct. 8 lesson can continue the same familiar object used in the earlier Carpentries Git session.

Use it to inspect history and repository state before substantive work moves to BUILD. During the collaboration exercise, learner-owned repositories can carry the recipe forward through a meaningful commit, push/pull, a deliberate same-line conflict, human resolution, and history review.

**Teaching line:** Git can tell us that two versions of guacamole exist. Git cannot tell us which guacamole tastes better.

**Commit-message prompt:** "Six months from now, will this message tell another person why this version exists?"
