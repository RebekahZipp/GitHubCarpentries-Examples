# TRY prompts

Use these prompts in your local clone before the shared BUILD.

## 1. Locate

```bash
pwd
git rev-parse --show-toplevel
```

**TALK:** What is the difference between your shell location and the repository root?

## 2. Observe

```bash
git status
git log --oneline
git remote -v
```

**TALK:** What does each command tell us that the others do not?

## 3. Find the BUILD artifact

```bash
ls
ls build-example
cat build-example/books.md
git status
```

**TALK:** What meaningful change could a person make to this file?

Do not make the change yet if the class has not reached the BUILD checkpoint.

## 4. Read the relationship

```bash
git remote -v
```

**TALK:** Why could you clone this public repository before Rebekah invited you as a collaborator?

Then ask:

> What will collaborator access change?

Expected distinction:

- public access lets you read and clone;
- your local clone lets you make local commits;
- collaborator write access lets your account push to the shared GitHub repository.

## 5. BUILD after the break

After Rebekah has collected your **GitHub username only**, invited you, and you have accepted the invitation:

```text
PULL -> CHANGE -> INSPECT -> ADD -> COMMIT -> REVIEW -> PUSH
```

Work in `build-example/books.md`.

Remember:

**COMMITTED != PUSHED**

Never share a password, token, recovery code, or other authentication secret.

## 6. When shared histories diverge

Read the evidence before fixing anything.

A rejected push does not necessarily mean there is a merge conflict. Pull/integrate the remote work first. If Git cannot automatically reconcile overlapping changes, then it will report a conflict and preserve the competing content for a human decision.

Use `guacamole.md` when the instructor directs the controlled conflict exercise.
