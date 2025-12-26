# Balancer Robot Workspace

## Overview
This repository serves as the central management hub (Manifest) for the Balancer Robot project. It utilizes the `west` tool to synchronize the firmware, desktop application, and the Zephyr RTOS environment into a unified development workspace.

## System Architecture
The project is divided into three primary domains:
1. **Control (Firmware):** Zephyr-based C++ application managing real-time PID loops and IMU fusion.
2. **Interface (Desktop App):** Python/C++ application for telemetry visualization and remote calibration.
3. **Infrastructure (Manifest):** Version pinning, documentation (PRD/ADR), and environment orchestration.

## Workspace Initialization

### Prerequisites
- Python 3.10+
- West (Zephyr's meta-tool)
- Zephyr SDK

### Setup
```bash
# Initialize workspace
west init -m https://github.com/royyandzakiy/balancer-robot-workspace-manifest.git balancer-robot-workspace
cd balancer-robot-workspace

# Synchronize repositories
west update

# Install python dependencies
pip install -r zephyr/scripts/requirements.txt

```

## Documentation Hierarchy

Project governance is managed via the `docs/` directory within this repository to maintain a single source of truth for design decisions.

| Directory | Content Type | Purpose |
| --- | --- | --- |
| `docs/prd/` | Product Requirements | Functional and non-functional specifications. |
| `docs/adr/` | Architecture Decisions | Records of technical trade-offs and justifications. |
| `docs/rfc/` | Proposals | Future feature designs and community feedback. |
| `docs/roadmap.md` | Strategic Planning | Project milestones and development backlog. |

## Licensing

Project specific licenses are located within their respective repositories.