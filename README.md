# GAE Rehosting Final Report

This repository contains the final report source and supporting documentation for the Cloud Computing final project: **Rehosting GAMA Animation Engine (GAE)**.

## Project Overview

The project focuses on improving the accessibility of GAE, a native Windows desktop application, by rehosting it in a cloud-based environment. Instead of requiring users to install GAE locally on a Windows machine, the application is deployed on a Windows EC2 instance and accessed through a web browser using Apache Guacamole.

## Main Goal

The main goal is to solve the accessibility limitation of a native Windows desktop application by enabling:

- cross-platform access,
- browser-based usage,
- no local installation for end users,
- centralized execution on a Windows cloud server.

## Architecture

```text
User Browser
    -> Apache Guacamole on Linux EC2
    -> RDP Connection
    -> Windows EC2 running GAE
```

## Related Repositories

- Original GAE/Gamatutor application: https://github.com/gamatutor/gamatutor
- Deployment configuration repository: https://github.com/EarlyOcean/cloud-computing-final-project

## Repository Contents

```text
.
├── README.md
├── report/
│   └── gae_rehosting_final_report.tex
├── docs/
│   ├── ai-declaration.md
│   ├── deployment-steps.md
│   ├── weekly-progress.md
│   └── video-links.md
└── .gitignore
```

## Notes

The final report follows the IEEE conference paper format and the IMRAD structure: Abstract, Introduction, Methods, Results, Discussion, Conclusion, and References.

The project does not redesign GAE as a cloud-native web application. Instead, it rehosts the original Windows desktop application into a cloud environment and exposes it through browser-based remote access.
