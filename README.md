# GitHub Carpentries Examples

This is the shared teaching repository for the OSU Libraries Git & GitHub workshop on Oct. 8, 2026.

The class uses one common repository so we can see the difference between a **public repository**, a **local clone**, a **local commit**, and **shared GitHub history**.

## During class

- **DEMO + DO:** Rebekah makes one small move and learners make the same move, then everyone stops to read the evidence.
- **TRY:** inspect, predict, or safely repeat a move in your local clone.
- **BUILD:** make a meaningful change to `build-example/books.md` in your local clone.
- **TALK:** explain what Git says, ask a question, or share an observation.

The repository is public, so you can clone it without collaborator access.

Before the first learner push, Rebekah will ask for your **GitHub username only** and invite you as a collaborator. Never share a password, access token, recovery code, or other authentication secret.

```text
CLONE       local copy       public access is enough
COMMIT      local history    happens on your computer
PUSH        shared history   GitHub write permission is required
```

## Clone and investigate

Choose where you want the repository to live, then:

```bash
git clone https://github.com/RebekahZipp/GitHubCarpentries-Examples.git
cd GitHubCarpentries-Examples
pwd
git rev-parse --show-toplevel
git status
git log --oneline
git remote -v
ls
```

Before changing anything, ask:

1. Where am I?
2. What repository am I in?
3. What branch am I on?
4. What history arrived with the clone?
5. What does `origin` point to?
6. Is my working tree clean?

## BUILD: Books I Have Read

The common class artifact is:

```text
build-example/
├── README.md
└── books.md
```

After collaborator access is accepted, the class practices the Carpentries collaboration rhythm:

**PULL -> CHANGE -> INSPECT -> ADD -> COMMIT -> REVIEW -> PUSH**

A useful change is to add a book you have read, a rating, or a short note. Git can record the change. It cannot decide whether your opinion is correct.

**COMMITTED != PUSHED.** A commit records history in your local clone. Push attempts to share recorded commits with GitHub.

## Conflict continuity: guacamole

`guacamole.md` carries forward the familiar Carpentries example. We can use it for a deliberate same-line conflict when we need to see what Git does when it cannot reconcile overlapping changes automatically.

A rejected push is **not automatically a merge conflict**. A rejected push can mean GitHub has history your local clone does not yet have. A merge conflict occurs when Git cannot automatically reconcile changes during integration.

**Teaching line:** Git can tell us that two versions of guacamole exist. Git cannot tell us which guacamole tastes better.

## Repository context

The repository also contains:

- `.gitignore` for intentional exclusions;
- `LICENSE` for reuse permission;
- `CITATION.cff` for citation metadata; and
- `TRY_PROMPTS.md` for short investigation prompts.

No library dataset or library-analysis example is needed for this workshop.

## Reasoning rhythms

Normal work:

**CHANGE -> INSPECT -> CHOOSE -> RECORD -> REVIEW -> SHARE**

When something surprises you:

**EXPECT -> OBSERVE -> EXPLAIN -> TEST -> ACT -> VERIFY**

The commands may change. The reasoning should become familiar.
