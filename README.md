# Practical automation and monitoring

I build small tools for document workflows, local automation and sensor monitoring. I focus on predictable behavior, clear failure messages and tests that run with synthetic data.

Start with these three projects:

- **[UndoWeave](https://github.com/Jgolding1998/undoweave):** undo one recorded agent edit while keeping separate later work. Its hardest problem is deciding when an undo is ambiguous enough to refuse. The [merge contract](https://github.com/Jgolding1998/undoweave/blob/main/docs/CONTRACT.md) explains that choice, including a real repeated-line bug found and fixed after the initial release. Try the disposable demo with no API key.
- **[Surface Map](https://github.com/Jgolding1998/surface-map):** turn website evidence into routes, a reviewable agent brief, or a PR change report. Its [comparison with REA](https://github.com/Jgolding1998/surface-map/blob/main/docs/REA_COMPARISON.md) shows both useful results and what a bounded static inventory misses.
- **[Jarvis Workbench](https://github.com/Jgolding1998/jarvis-workbench):** practice a local workstation companion before enabling devices. The [architecture](https://github.com/Jgolding1998/jarvis-workbench/blob/main/docs/ARCHITECTURE.md) separates observations, policy decisions and physical actions so an attractive dashboard cannot silently grant permissions.

I use Claude Code and Codex in development. The repositories document concrete
choices, reproducible checks and remaining limits so the work can be evaluated
from the code and behavior.

| Project | What it does | Engineering focus |
| --- | --- | --- |
| [UndoWeave](https://github.com/Jgolding1998/undoweave) | Selective undo for recorded coding-agent edits, with a readable timeline | Conservative conflict refusal, durable recovery and preservation of Git state |
| [Jarvis Workbench](https://github.com/Jgolding1998/jarvis-workbench) | A local presence and hand-control dashboard, guided setup and optional text chat | Device ownership, permission boundaries and state transitions |
| [PDF Renamer Local](https://github.com/Jgolding1998/pdf-renamer-local) | Preview invoice filenames and download the renamed PDFs as a ZIP | Bounded parser processes, safe filenames and preview consistency |
| [Thermal Watch](https://github.com/Jgolding1998/thermal-watch) | Monitor simulated or CSV temperature readings | Sensor freshness, hysteresis, event history and optional webhook delivery |
| [Repo Preflight](https://github.com/Jgolding1998/repo-preflight) | Check files and reachable Git history before publishing | Redacted findings, narrow exceptions and CLI exit contracts |
| [Site Contract API](https://github.com/Jgolding1998/site-contract-api) | Extract static HTML into a JSON endpoint using explicit rules | Required fields, drift detection and restricted remote sources |
| [Surface Map](https://github.com/Jgolding1998/surface-map) | Inspect saved web captures and selected source files without running them | Syntax and scope analysis, evidence labels and value-free API skeletons |
| [Presence Guard](https://github.com/Jgolding1998/presence-guard) | A standalone camera presence guard with optional Windows locking | Local processing, timed policies and explicit action permissions |
| [Swarm Evolution](https://github.com/Jgolding1998/swarm-evolution) | A space shooter with inherited enemy traits, campaigns and endless play | Seeded simulation, constrained evolution and visible fitness |
| [Barricade Defense](https://github.com/Jgolding1998/barricade-defense) | Build and upgrade a defense in campaigns or endless survival | Shared resources, path invariants and tested strategy bots |
| [YouTube File Kit](https://github.com/Jgolding1998/youtube-file-kit) | A local yt-dlp front end for public-video downloads | Restricted extraction, bounded jobs and clear failure states |
| [MP4 Audio Kit](https://github.com/Jgolding1998/mp4-audio-kit) | Drop MP4 files and download MP3 audio, with ZIP batches | Isolated conversion, filename handling and automatic cleanup |

[Try the Jarvis setup planner](https://jarvis-workbench.jrgoldin.chatgpt.site). You can plan on a phone, then continue on a computer for desktop features. Each repository includes setup commands, tests and practical limits. Hardware and external integrations need the operator's own configuration and manual checks.

<a href="https://github.com/Jgolding1998/jarvis-workbench"><img src="https://raw.githubusercontent.com/Jgolding1998/jarvis-workbench/main/docs/dashboard.png" alt="Jarvis Workbench demo dashboard" width="49%"></a>
<a href="https://github.com/Jgolding1998/thermal-watch"><img src="https://raw.githubusercontent.com/Jgolding1998/thermal-watch/main/docs/dashboard.png" alt="Thermal Watch demo dashboard" width="49%"></a>

## Feedback

[Leave a suggestion, like, dislike or problem report](https://github.com/Jgolding1998/Jgolding1998/issues/new?template=feedback.yml), or [browse the feedback board](https://github.com/Jgolding1998/Jgolding1998/issues?q=is%3Aissue%20label%3Afeedback). Feedback is public. Do not include API keys, names, email addresses, private documents or unredacted logs.

## Security

For suspected vulnerabilities, use the affected project's private reporting option. [Security policies and reporting links for every project](https://github.com/Jgolding1998/Jgolding1998/blob/main/SECURITY.md) are listed separately from public feedback.

