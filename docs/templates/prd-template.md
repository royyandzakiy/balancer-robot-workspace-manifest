# PRD [ID]: [Feature/Product Name]

* **Status**: [Draft | Review | Approved | Deprecated]
* **Owner**: [Your Name]
* **Version**: 1.0.0

## 1. Executive Summary
[A high-level pitch of what this product/feature is and why it matters.]

## 2. Goals & Objectives
* [Goal 1, e.g., Create a stable 2-wheeled platform.]
* [Goal 2, e.g., Demonstrate sub-10ms latency in control loops.]

## 3. Target User / Use Case
[Who is this for? e.g., "Embedded developers wanting a mobile testing platform."]

## 4. Functional Requirements
| ID | Requirement | Priority | Description |
| :--- | :--- | :--- | :--- |
| FR1 | Self-Balancing | P0 | Must remain upright without external support. |
| FR2 | Remote Control | P1 | Control via Bluetooth/Wi-Fi using Desktop App. |
| FR3 | Safety Cutoff | P0 | Motors must disable if tilt angle exceeds 45°. |

## 5. Non-Functional Requirements (Technical Constraints)
* **Performance**: Control loop must run at [X] Hz.
* **Portability**: Must be flashable to [nRF52840 / ESP32] via Zephyr.
* **Battery**: Must operate for [X] hours on a single charge.

## 6. Success Metrics
[How do we know we "won"? e.g., "Robot stays upright for 15 minutes straight."]

## 7. Out of Scope
[What are we NOT building yet? e.g., "Obstacle avoidance is for V2."]