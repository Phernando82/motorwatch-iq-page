# MotorWatch IQ — Portfolio Page

![HTML5](https://img.shields.io/badge/HTML5-CSS3-E34F26?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=flat&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-Live-222222?style=flat&logo=githubpages&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-a6e3a1?style=flat)
![i18n](https://img.shields.io/badge/i18n-EN_%2F_ES-89b4fa?style=flat)

Portfolio presentation page for the MotorWatch IQ project — a full-stack IIoT motor condition monitoring system.

🌐 **Live:** https://phernando82.github.io/motorwatch-iq-page/

---

## About

This is a single-page portfolio site documenting the MotorWatch IQ project across 6 sections. It is built with plain HTML/CSS and vanilla JavaScript — no framework, no build step, zero dependencies beyond Google Fonts.

The visual identity mirrors the MotorWatch IQ application itself: Catppuccin Mocha dark palette, IBM Plex Mono/Sans typography, and the same accent colours used throughout the PySide6 UI, Grafana dashboards, and generated maintenance reports.

---

## Sections

| # | Section | Content |
|---|---------|---------|
| 01 | **Hardware** | Physical control panel, HMI screens, TIA Portal screenshots, alarm logic documentation |
| 02 | **Simulator** | PySide6 desktop app screenshots, technical design decisions |
| 03 | **Communication** | IIoT data pipeline architecture, OPC UA / MQTT / InfluxDB stack |
| 04 | **Analytics** | Grafana dashboards, embedded bilingual maintenance report |
| 05 | **Intelligence** | ML pipeline: Isolation Forest, trend analysis, CWRU fault classification |
| 06 | **About** | Engineer profile, skills, repository links |

---

## Technical Details

- **No framework** — plain HTML5 + CSS3 + vanilla JS
- **Bilingual EN/ES** — full page translation via `data-en` / `data-es` attributes and `body.lang-en/es` class toggle
- **Boot console animation** — CSS `@keyframes` with `nth-child` delays simulate service startup sequence; LED dots animate from grey → yellow → green via JS `data-state` attributes after all lines appear
- **Embedded report** — live bilingual HTML maintenance report in `<iframe>`; language toggle inside the report itself
- **Dark sidebar design** — Catppuccin Mocha `#0d0d14` background with `#1e293b` sidebar, consistent with the application palette
- **Responsive** — single breakpoint at 900px, grid layouts collapse to single column

---

## Repository Structure

```
motorwatch-iq-page/
├── index.html
├── images/
│   ├── board.jpg                    # Physical control panel
│   ├── hmi_main.jpg                 # HMI pre-alarm state
│   ├── hmi_alarm.jpg                # HMI alarm state
│   ├── hmi_settings.jpeg            # HMI settings menu
│   ├── hmi_threshold_settings.jpg   # HMI threshold configuration
│   ├── launcher.png                 # PySide6 launcher tab
│   ├── simulator.png                # PySide6 simulator tab
│   ├── analytics.png                # PySide6 analytics tab
│   ├── settings.png                 # PySide6 settings tab
│   ├── sensors_grafana.png          # Grafana sensor dashboard
│   ├── analytics_grafana.png        # Grafana anomaly dashboard
│   ├── network_view.png             # TIA Portal network view
│   ├── project_tree.png             # TIA Portal project tree
│   ├── fb_evaluate.png              # FB_Evaluate_Motor SCL
│   ├── fb_save_parameters.png       # FB_Save_Parameters SCL
│   ├── output_alarm.png             # Main OB1 alarm ladder
│   └── main_screen.png              # HMI WinCC editor
└── reports/
    ├── motorwatch_report_EN.html
    └── motorwatch_report_ES.html
```

---

## Related Repositories

| Repository | Description |
|-----------|-------------|
| [motor_watch_IQ](https://github.com/Phernando82/motor_watch_IQ) | Python application — full IIoT stack |
| [motorwatch-iq-plc-hmi](https://github.com/Phernando82/motorwatch-iq-plc-hmi) | TIA Portal V20 — PLC & HMI project |

---

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*Developed by [Fernando Valverde](https://github.com/Phernando82) · [LinkedIn](https://www.linkedin.com/in/fernandos-valverde/)*
