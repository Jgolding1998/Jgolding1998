# Research and design references

These projects are small original implementations. The repositories below informed the problem selection and review checklist; their source code has not been copied into these projects.

| Reference | Useful idea | Applied here |
| --- | --- | --- |
| [Home Assistant](https://github.com/home-assistant/core) | Local control and explicit device state | Thermal Watch separates normal, pending, fault, and stale states |
| [ESPHome](https://github.com/esphome/esphome) | Hardware adapters separated from application behavior | Thermal Watch has simulated input, a CSV contract, and a DS18B20 producer |
| [Stirling-PDF](https://github.com/Stirling-Tools/Stirling-PDF) | Practical document workflows with a self-hosted option | PDF Renamer Local has a focused preview and export workflow |
| [Gitleaks](https://github.com/gitleaks/gitleaks) | A dedicated secret scanner should be part of repository review | Repo Preflight complements a Gitleaks scan and documents its own gaps |
| [changedetection.io](https://github.com/dgtlmoon/changedetection.io) | Change events are more useful than repeated status messages | Temperature alerts use dwell time, hysteresis, and cooldowns |

## Decisions worth inspecting

**Keep side effects behind explicit permissions.** Jarvis starts disarmed and simulated. Enabling a camera is separate from allowing a real workstation lock or opening the sample spreadsheet. Person counting does not identify anyone.

**Make the demo useful without access to private systems.** The projects use synthetic documents and sensor values. No employer data, private integrations, logs, browser sessions, or account credentials are needed.

**Show failure in the interface.** A disconnected sensor is a fault to investigate. A camera that stops delivering frames cannot be treated as proof that the desk is empty. A parsing error is attached to the affected document.

**Keep writing tied to evidence.** Setup instructions include test commands. Hardware limits are stated separately. No invented deployment history, benchmark results, or coverage percentage is used.

## Further reading

- [GitHub: removing sensitive data](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository). A committed credential must be rotated; deleting a file does not revoke it or clean other clones.
- [GitHub: personal profiles](https://docs.github.com/en/account-and-profile/concepts/personal-profile). A profile README and selected repositories help visitors find the work worth reviewing.

Reviewed October 28, 2026.
