# ADR 0001: Use Zephyr RTOS for Balancer Robot Firmware

* **Status**: Accepted
* **Date**: 2025-12-26
* **Deciders**: @royyandzakiy

## Context and Problem Statement
The robot requires a highly modular firmware architecture that can easily be ported to different MCUs (Nordic, STM32) and requires a robust build system for multi-repo management.

## Decision Drivers
* Need for a powerful Meta-Build system (West).
* High-quality C++ support.
* Decoupling hardware (DeviceTree) from application logic.

## Decision Outcome
Chosen Option: **Zephyr RTOS**.
While ESP-IDF is excellent, Zephyr's hardware abstraction via DeviceTree and its `west` workspace management make it superior for a professional-grade, multi-repo project that may expand to non-Espressif hardware.