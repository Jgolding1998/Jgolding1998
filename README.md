# Practical automation and monitoring

Small systems that solve a concrete problem and make their behavior easy to inspect. The projects below include working demos, design decisions, failure handling, and automated tests that run without credentials or hardware.

| Project | Try it | Engineering focus |
| --- | --- | --- |
| [Jarvis Workbench](https://github.com/Jgolding1998/jarvis-workbench) | [Guided setup and gesture practice](https://jarvis-workbench.jrgoldin.chatgpt.site) | Local hand tracking, camera ownership, presence state machine, permission boundaries |
| [PDF Renamer Local](https://github.com/Jgolding1998/pdf-renamer-local) | Preview invoice filenames, then download a ZIP | Untrusted input, bounded parsing, safe filenames, collision handling, local document processing |
| [Thermal Watch](https://github.com/Jgolding1998/thermal-watch) | Watch a freezer and cooker drift outside their ranges | Sensor freshness, hysteresis, persistence, alert delivery, SQLite history |
| [Repo Preflight](https://github.com/Jgolding1998/repo-preflight) | Scan a working tree and reachable Git history | Redacted reporting, regression fixtures, exact exceptions, CLI exit contracts |
| [Site Contract API](https://github.com/Jgolding1998/site-contract-api) | Turn static HTML into a typed JSON endpoint | Explicit extraction contracts, drift detection, bounded parsing, restricted HTTPS sources |
| [Surface Map](https://github.com/Jgolding1998/surface-map) | Inspect saved HTML, HAR and JavaScript captures | Evidence labels, value-free schemas, API skeletons, capture comparison |

Run the checks yourself: [Jarvis CI](https://github.com/Jgolding1998/jarvis-workbench/actions), [PDF CI](https://github.com/Jgolding1998/pdf-renamer-local/actions), [temperature CI](https://github.com/Jgolding1998/thermal-watch/actions), [preflight CI](https://github.com/Jgolding1998/repo-preflight/actions).

<a href="https://github.com/Jgolding1998/jarvis-workbench"><img src="https://raw.githubusercontent.com/Jgolding1998/jarvis-workbench/main/docs/dashboard.png" alt="Jarvis Workbench demo dashboard" width="49%"></a>
<a href="https://github.com/Jgolding1998/thermal-watch"><img src="https://raw.githubusercontent.com/Jgolding1998/thermal-watch/main/docs/dashboard.png" alt="Thermal Watch demo dashboard" width="49%"></a>

## How to review the work

Start with a project's quick start, run its tests, and read its architecture notes. Each project separates a working local demo from the devices or services needed for live use. Optional integrations use the operator's own configuration. No shared AI account or embedded API key is provided.

Tests cover simulated failures and boundary cases. Camera accuracy, workstation locking, physical sensors, and real notification delivery require the manual checks described in the relevant project. Test results do not imply certification or production deployment.

