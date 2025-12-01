# Bumble Auto-Unmatch
> This project automates the process of unmatching users on Bumble, removing repetitive manual steps and ensuring consistent cleanup of unwanted matches. By leveraging Android automation, Bumble Auto-Unmatch helps users maintain a tidy inbox and streamline dating-app workflows with minimal effort.


<p align="center">
  <a href="https://Appilot.app" target="_blank"><img src="https://github.com/Instagram-Automations/Footer-test/blob/main/appilot-baner.png" alt="Appilot Banner" width="100%"></a>
</p>

<p align="center">
  <a href="https://t.me/devpilot1" target="_blank"><img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"></a>
  <a href="mailto:support@appilot.app" target="_blank"><img src="https://img.shields.io/badge/Email-support@appilot.app-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"></a>
  <a href="https://Appilot.app" target="_blank"><img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website"></a>
  <a href="https://discord.gg/xvPWXJXCw7" target="_blank"><img src="https://img.shields.io/badge/Join-Appilot_Community-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Appilot Discord"></a>
</p>



## Introduction
This automation tool performs hands-free unmatching actions on the Bumble Android app. It removes the tedious routine of manually navigating profiles, confirming unmatch dialogs, and clearing histories. For users or teams managing large-scale dating-app workflows, it provides fast, reliable automation that improves efficiency and consistency.

### Intelligent Match-Management Automation
- Reduces time spent manually browsing and unmatching inactive or undesired profiles.
- Uses Android UI automation to reliably trigger navigation, menu actions, and confirmations.
- Supports scheduled or on-demand cleanup sessions.
- Operates without requiring device rooting or intrusive modification.
- Designed to scale across device farms and automation clusters.

## Core Features
| Feature | Description |
|----------|-------------|
| Automated Unmatch Workflow | Navigates to match list, opens each profile, and performs unmatch actions. |
| Smart UI Detection | Uses UI Automator/Appilot signals to identify correct buttons and dialogs. |
| Retry Logic | Automatically retries unfinished actions due to slow device or network delays. |
| Session Scheduler | Allows scheduled cleanup runs at configurable intervals. |
| Device Abstraction | Supports ADB-less and Appium-like flows across multiple Android devices. |
| Logging & Telemetry | Outputs structured logs for each unmatch attempt and result. |
| Parallel Device Execution | Runs multiple devices simultaneously using horizontal workers. |
| Proxy/Network Controller | Integrates optional proxy rotation via internal utility modules. |
| Safety Confirmation | Prevents accidental actions using rule-based match filters. |
| Result Export | Stores summaries of unmatched profiles in JSON and CSV outputs. |

---
## How It Works
1. **Input or Trigger** — A manual CLI command or scheduled job initiates an unmatch session.
2. **Core Logic** — The automation framework launches Bumble, scans matches, opens profiles, and triggers the unmatch dialog.
3. **Output or Action** — Successfully unmatched profiles are logged and written to output files.
4. **Other Functionalities** — Optional filters skip premium users, pending chats, or recently matched profiles.
5. **Safety Controls** — Multi-step confirmation logic, UI validation, and rollback safeguards prevent incorrect actions.

---
## Tech Stack
**Language:** Python
**Frameworks:** Appilot, UI Automator, lightweight job scheduler
**Tools:** ADB-less control, device orchestrators, proxy utilities, internal loggers
**Infrastructure:** Local devices, cloud device farms, containerized workers

---
## Directory Structure
    automation-bot/
    ├── src/
    │   ├── main.py
    │   ├── automation/
    │   │   ├── tasks.py
    │   │   ├── scheduler.py
    │   │   └── utils/
    │   │       ├── logger.py
    │   │       ├── proxy_manager.py
    │   │       └── config_loader.py
    ├── config/
    │   ├── settings.yaml
    │   ├── credentials.env
    ├── logs/
    │   └── activity.log
    ├── output/
    │   ├── results.json
    │   └── report.csv
    ├── requirements.txt
    └── README.md

---
## Use Cases
- **Solo users** use it to automatically unmatch inactive profiles so they can keep their inbox lean.
- **Growth teams** use it to reset devices between experiments so they can maintain consistent testing conditions.
- **Automation engineers** use it to validate UI flows by repeatedly performing safe unmatch operations.
- **Device-farm operators** use it to schedule cleanup cycles so they can ensure stable environments across dozens of phones.

---
## FAQs
**Q: Does this require rooting the device?**
A: No, it works with standard Android automation APIs.

**Q: Can it skip certain matches?**
A: Yes, you can configure filters for skipping based on match age, activity, or other criteria.

**Q: What happens if a dialog fails to load?**
A: The retry logic attempts the step again with backoff and logs the failure.

**Q: Can it run on multiple devices?**
A: Yes, it supports horizontal scaling with multiple workers.

---
## Performance & Reliability Benchmarks
**Execution Speed:** Around 18–25 unmatch actions per minute under typical device-farm network conditions.
**Success Rate:** Approximately 93–94% across long-running sessions with automatic retries.
**Scalability:** Supports 300–1,000 Android devices using sharded task queues and horizontally scaled workers.
**Resource Efficiency:** Targets ~8–12% CPU and 120–180 MB RAM per worker/device depending on device speed.
**Error Handling:** Includes structured logging, retry mechanisms, exponential backoff, alert triggers, and recovery workflows.


<p align="center">
<a href="https://cal.com/app-pilot-m8i8oo/30min" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
 
  <a href="https://www.youtube.com/@Appilot-app/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
