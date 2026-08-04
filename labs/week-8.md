# 🗓️ Week 8 — The Broken Ledger Hotfix

> **CMU Topic:** Git Fundamentals  
> **Difficulty:** ⭐⭐⭐⭐⭐⭐⭐⭐ (7.5 / 10)  
> **Estimated Time:** 4 Hours  
> **Expected Failed Attempts:** 6–10

---

# 📖 Engineering Story

An emergency production hotfix was pushed directly to the **main** branch minutes before market open.

Three engineers committed conflicting changes.

One developer force-pushed an outdated branch.

Another accidentally committed sensitive financial configuration files.

The production repository has diverged, deployment pipelines are failing, and no one knows which version represents the correct system state.

---

# 💼 Business Impact

Restores the integrity of the production source repository before the next deployment window, preventing financial transaction failures and preserving the complete engineering audit trail.

---

# 📚 Concepts Used

- Repository initialization
- Staging area
- Commits
- Commit history
- Branches
- Merging
- Merge conflicts
- Git logs
- Git diff
- Repository state inspection

---

# 📊 Lab Statistics

| Property | Value |
|-----------|-------|
| Folder Complexity | **Multi-branch enterprise Git repository** |
| Number of Files | **110** |
| Hidden Files | **1 (.git)** |
| Decoy Files | **15** |
| Intentional Bugs | **6** |
| Investigation Level | **High Code Collision** |

---

# 🎯 Main Mission

Recover the production repository by:

- Identifying the correct branch.
- Inspecting commit history.
- Recovering missing changes.
- Resolving merge conflicts.
- Removing accidental commits.
- Producing a deployable repository without losing legitimate engineering history.

---

# ⭐ Bonus Mission

Perform a **manual three-way merge** while preserving every valid production change and maintaining a clean, understandable commit history.

---

# ⚠️ Typical Beginner Mistakes

- Committing directly to the wrong branch.
- Resolving merge conflicts by deleting large sections of code.
- Forgetting to inspect `git diff` before committing.
- Creating unnecessary merge commits.
- Losing work through improper checkout operations.
- Treating Git as file storage instead of version history.

---

# 🏭 Real Production Equivalent

**GitHub Release Engineering**

Recovering production repositories after failed hotfix deployments, conflicting feature branches, and emergency release patches.

---

# ✅ Mastery Criteria

To successfully complete this laboratory, the student should demonstrate:

- Complete understanding of repository state.
- Correct conflict resolution.
- Clean commit history.
- Safe branching workflow.
- No accidental code loss.
- Deployable production repository.

---

# 🧠 Productive Struggle Profile

| Metric | Value |
|---------|-------|
| Challenge Rating | **7.5 / 10** |
| CS50 Equivalent | **Pset 8 (Homepage / Trivia)** — Multiple independent components must be integrated into one working system without breaking existing functionality. |
| Hours of Productive Struggle | **4 Hours** |
| Average Debugging Time | **1.5 Hours** |
| Independent Research | **Moderate** — Understanding branching strategies, merge mechanics, and repository history visualization. |
| Man Page Utilization | **Moderate** — Exploring commit inspection, branching workflows, merge behavior, and repository status commands. |

---

# 🎓 Learning Outcome

After completing this laboratory, you should be able to:

- Navigate Git repositories confidently.
- Create meaningful commits.
- Manage feature branches.
- Resolve merge conflicts safely.
- Read repository history effectively.
- Understand how production teams collaborate using Git.
- Recover from common version-control mistakes without losing work.

---

# 🚀 Industry Skills Gained

- Git Fundamentals
- Branching Strategies
- Merge Conflict Resolution
- Commit History Analysis
- Collaborative Development
- Release Engineering
- Version Control
- Production Repository Recovery

---

> ## 💡 Difficulty Philosophy
>
> This laboratory follows the **CS50 model**.
>
> The lecture introduces Git fundamentals such as commits, branches, logs, and merges.
>
> The laboratory combines these concepts into a realistic production incident where multiple developers have created conflicting histories under time pressure.
>
> The challenge is **not** remembering Git commands.
>
> The challenge is reconstructing the correct repository state, preserving engineering history, and making careful decisions that restore a deployable codebase without introducing new errors.
