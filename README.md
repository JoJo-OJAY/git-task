# git-task
My first Git assignment
# Git Task

## 1. What is Version Control?
Version control is a system that tracks changes to files over time, allowing you to recall specific versions later. It lets multiple people collaborate on a project, see the history of changes, and revert to earlier versions if something goes wrong. Examples of version control systems include Git, SVN, and Mercurial.

---

## 2. Difference Between Git and GitHub

| Git | GitHub |
|-----|--------|
| A version control tool installed on your computer | A cloud-based platform that hosts Git repositories |
| Works locally (offline) | Works online |
| Manages and tracks code history | Allows collaboration, pull requests, and code review |
| A command-line tool | Has a graphical web interface |

In short: **Git** is the tool, **GitHub** is the service built around it.

---

## 3. Three Alternatives to GitHub

1. **GitLab** - A DevOps platform with built-in CI/CD pipelines and self-hosting options.
2. **Bitbucket** - By Atlassian; integrates well with Jira and Trello for project management.
3. **Azure DevOps (Azure Repos)** - Microsoft's platform for enterprise-level Git hosting and pipelines.

---

## 4. Difference Between `git fetch` and `git pull`

| `git fetch` | `git pull` |
|-------------|------------|
| Downloads changes from the remote repository | Downloads **and** merges changes into your current branch |
| Does **not** affect your working files | Directly updates your working files |
| Safer — lets you review before merging | Faster but can cause merge conflicts |

**In simple terms:**
- `git fetch` = "Check what changed remotely, but don't touch my files yet."
- `git pull` = "Get the changes and apply them to my branch now."

---

## 5. Git Rebase

**Git rebase** moves or replays your commits on top of another branch. Instead of creating a merge commit, it rewrites history to make it look like you branched off from a later point — resulting in a cleaner, linear history.

**Command:**
```bash
git rebase main
## 6. Git Cherry-Pick

**Git cherry-pick** lets you pick a specific commit from one branch and apply it
to another branch, without merging the entire branch.

Think of it like this: imagine you baked 10 cookies but only want to move
one specific cookie to a different plate — you don't move all the cookies,
just the one you want. That is exactly what cherry-pick does with commits.

**Command:**
```bash
git cherry-pick <commit-hash> 