# BUILD: Books I Have Read

This folder is the common BUILD artifact for the Oct. 8 workshop.

Everyone begins from the same repository history by cloning `RebekahZipp/GitHubCarpentries-Examples`. Each clone is a complete local Git repository. Learners can make local commits independently. During class, Rebekah adds learners as collaborators so they can also push to the shared GitHub repository.

## Before BUILD

You should be able to verify:

```bash
git status
git remote -v
git log --oneline
ls build-example
cat build-example/books.md
```

Before the break, Rebekah will ask for your **GitHub username only** and send a collaborator invitation. Do not share passwords, tokens, recovery codes, or other authentication secrets.

## Working rhythm

```text
PULL -> CHANGE -> INSPECT -> ADD -> COMMIT -> REVIEW -> PUSH
```

A typical cycle is:

```bash
git pull origin main
# edit build-example/books.md
git status
git diff
git add build-example/books.md
git diff --staged
git commit -m "Add a book to reading list"
git log --oneline
git show HEAD
git push origin main
```

Do not memorize the block as a magic recipe. Stop after each meaningful move and read what Git says.

## Choose a meaningful change

You can:

- add a book you have read;
- add a rating to an existing row; or
- add a short note.

Git can record that a rating or note changed. Git cannot decide whether the opinion is correct.

## Shared history

Everyone starts from the same history. Once learners make local commits, those histories can diverge.

Before pushing shared work, pay attention to what GitHub may have received from another learner.

**COMMITTED != PUSHED**

A rejected push is not automatically a merge conflict. Read the rejection, integrate newer remote work, and only call it a conflict if Git reports that it cannot automatically reconcile overlapping changes.
