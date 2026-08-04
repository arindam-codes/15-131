# 🗓️ Week 7 — The Shadow Network Detector

> **CMU Topic:** Automation with Bash  
> **Difficulty:** ⭐⭐⭐⭐⭐⭐⭐⭐ (8 / 10)  
> **Estimated Time:** 5 Hours  
> **Expected Failed Attempts:** 10–15

---

# 📖 Engineering Story

Persistent cryptomining malware penetrates an unsecured testing instance, injecting obfuscated cron configurations and spawning hidden background processes that silently exfiltrate company data through hijacked system network sockets. :contentReference[oaicite:0]{index=0}

---

# 💼 Business Impact

Reclaims hijacked infrastructure compute resources and immediately shuts down active data exfiltration channels before they spread through the engineering environment. :contentReference[oaicite:1]{index=1}

---

# 📚 Concepts Used

- Cron scheduling
- Process tracking
- Background processing (`&`, `nohup`)
- Job management
- Signal handling
- Script trap routines

:contentReference[oaicite:2]{index=2}

---

# 📊 Lab Statistics

| Property | Value |
|-----------|-------|
| Folder Complexity | **Standard Linux directory layouts with hidden cron entries** |
| Number of Files | **65** |
| Hidden Files | **12** |
| Decoy Files | **40** |
| Intentional Bugs | **4** |
| Investigation Level | **Multi-process Obfuscation** |

:contentReference[oaicite:3]{index=3}

---

# 🎯 Main Mission

Audit the active process space.

Trace hidden parent execution origins.

Write an automated cleanup tool that intercepts process signals and cleans temporary files safely upon script interruption. :contentReference[oaicite:4]{index=4}

---

# ⭐ Bonus Mission

Construct a persistent monitoring loop using **cron** that automatically detects and terminates unauthorized background processes within moments of their initial execution. :contentReference[oaicite:5]{index=5}

---

# ⚠️ Typical Beginner Mistakes

- Killing processes blindly without inspecting parent-child relationships.
- Missing hidden persistence through cron jobs.
- Forgetting to clean temporary resources when scripts terminate unexpectedly.
- Leaving zombie or orphaned processes running after interruption.

:contentReference[oaicite:6]{index=6}

---

# 🏭 Real Production Equivalent

**CrowdStrike Incident Response Operations**

Tracking, isolating, and neutralizing active malware execution chains and persistent adversarial footholds inside production Linux infrastructure. :contentReference[oaicite:7]{index=7}

---

# ✅ Mastery Criteria

To successfully complete this laboratory, the student should demonstrate:

- Complete removal of malicious background processes.
- Correct identification of persistence mechanisms.
- Reliable process monitoring.
- Robust signal trapping.
- Proper cleanup during unexpected termination.
- Zero lingering malware execution paths.

:contentReference[oaicite:8]{index=8}

---

# 🧠 Productive Struggle Profile

| Metric | Value |
|---------|-------|
| Challenge Rating | **8 / 10** |
| CS50 Equivalent | **Pset 7 (Fiftyville)** — High-stakes forensic investigation where multiple independent clues must be connected to reconstruct hidden execution paths. |
| Hours of Productive Struggle | **5 Hours** |
| Average Debugging Time | **2.5 Hours** |
| Independent Research | **Very High** — Tracking hidden persistent scripts, process parent hierarchies, background execution, and operational environment traps. |
| Man Page Utilization | **High** — Studying process inspection, scheduling systems, signal handling, asynchronous execution, and job-control utilities. |

:contentReference[oaicite:9]{index=9}

---

# 🎓 Learning Outcome

After completing this laboratory, you should be able to:

- Inspect and understand Linux process trees.
- Manage foreground and background jobs safely.
- Create resilient automation using `cron`.
- Handle Unix signals correctly.
- Build scripts that clean up resources using traps.
- Diagnose process persistence and scheduled execution.
- Think like a production incident responder when investigating compromised systems.

---

# 🚀 Industry Skills Gained

- Bash Automation
- Process Management
- Job Control
- Signal Handling
- Cron Scheduling
- Linux Incident Response
- Malware Investigation
- Production Infrastructure Monitoring

---

> ## 💡 Difficulty Philosophy
>
> This laboratory follows the **CS50 model**.
>
> The lecture introduces process management, scheduling, and signal handling.
>
> The laboratory combines those ideas into a realistic production incident where malicious software uses cron jobs, hidden background processes, and persistence mechanisms to evade detection.
>
> The challenge is not remembering Bash syntax.
>
> The challenge is learning to reason about asynchronous execution, process ancestry, cleanup routines, and persistence mechanisms under realistic engineering constraints until the entire execution chain is understood and safely removed.
