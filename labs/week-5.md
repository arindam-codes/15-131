# 🗓️ Week 5 — The Automated Infrastructure Health Check

> **CMU Topic:** Bash Scripting  
> **Difficulty:** ⭐⭐⭐⭐⭐⭐⭐ (7 / 10)  
> **Estimated Time:** 4 Hours  
> **Expected Failed Attempts:** 7–12

---

# 📖 Engineering Story

A cluster of bare-metal storage frames randomly throws **kernel memory soft-locks** and **run-away file table allocations**, bringing database engines to an immediate halt. :contentReference[oaicite:0]{index=0}

---

# 💼 Business Impact

Eradicates intermittent node failures and preserves automated **high-frequency order book replication states**. :contentReference[oaicite:1]{index=1}

---

# 📚 Concepts Used

- System variables
- Positional parameters
- Conditional blocks
- Structural loops
- File-test operators
- Exit statuses

:contentReference[oaicite:2]{index=2}

---

# 📊 Lab Statistics

| Property | Value |
|-----------|-------|
| Folder Complexity | **Standardized monitoring root filesystem structure** |
| Number of Files | **12** |
| Hidden Files | **1** |
| Decoy Files | **4** |
| Intentional Bugs | **5** |
| Investigation Level | **Complex System States** |

:contentReference[oaicite:3]{index=3}

---

# 🎯 Main Mission

Build a **portable, error-resilient automation script** that:

- Verifies disk allocations.
- Flags resource leaks.
- Detects unhealthy system states.
- Handles failures safely.
- Returns meaningful exit codes.

The script must execute correctly across arbitrary Linux environments without manual modification. :contentReference[oaicite:4]{index=4}

---

# ⭐ Bonus Mission

Extend the monitoring utility to:

- Parse complex command-line switches.
- Accept positional parameters.
- Generate a formatted **Markdown operational health report** dynamically after every execution.

:contentReference[oaicite:5]{index=5}

---

# ⚠️ Typical Beginner Mistakes

- Forgetting to quote variables, causing unwanted word splitting.
- Mishandling exit codes.
- Creating accidental infinite loops.
- Assuming filenames never contain spaces.
- Failing to validate input parameters before execution.

:contentReference[oaicite:6]{index=6}

---

# 🏭 Real Production Equivalent

**Amazon EC2 Fleet Diagnostics**

Writing lightweight host-level diagnostic monitors across large auto-scaling infrastructure fleets. :contentReference[oaicite:7]{index=7}

---

# ✅ Mastery Criteria

To successfully complete this laboratory, the student should demonstrate:

- Flawless execution across arbitrary environments.
- Graceful handling of edge cases.
- Robust parameter validation.
- Reliable conditional logic.
- Proper exit status handling.
- Portable Bash scripting with predictable behavior.

:contentReference[oaicite:8]{index=8}

---

# 🧠 Productive Struggle Profile

| Metric | Value |
|---------|-------|
| Challenge Rating | **7 / 10** |
| CS50 Equivalent | **Pset 5 (Speller)** — Transitioning from data exploration to robust, memory-safe system programming. |
| Hours of Productive Struggle | **4 Hours** |
| Average Debugging Time | **2 Hours** |
| Independent Research | **High** — Debugging edge cases involving word splitting, parameter expansion, and unexpected shell environment behavior. |
| Man Page Utilization | **Very High** — Systematic exploration of conditional operators, test primitives, and control-flow mechanics. |

:contentReference[oaicite:9]{index=9}

---

# 🎓 Learning Outcome

After completing this laboratory, you should be able to:

- Write portable Bash scripts.
- Use positional parameters effectively.
- Design reliable conditional logic.
- Build reusable automation tools.
- Handle failures using meaningful exit codes.
- Validate files, directories, and execution environments safely.
- Produce operational reports directly from shell scripts.

---

# 🚀 Industry Skills Gained

- Bash Automation
- Infrastructure Health Monitoring
- Portable Shell Scripting
- Systems Diagnostics
- Fleet Monitoring
- Linux Operations
- Production Reliability
- Automation Engineering

---

> ## 💡 Difficulty Philosophy
>
> This laboratory follows the **CS50 model**.
>
> The lecture teaches Bash scripting primitives such as variables, loops, conditionals, and exit codes.
>
> The laboratory forces you to combine those primitives into a **production-grade monitoring utility** that behaves correctly under unpredictable environments and failure conditions.
>
> The challenge is not remembering Bash syntax.
>
> The challenge is engineering a resilient automation tool that survives malformed input, unexpected system states, and edge cases while remaining portable, maintainable, and reliable.
```
