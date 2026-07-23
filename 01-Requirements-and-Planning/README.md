# 01 - Requirements and Planning

This directory contains the business, technical, operational, and wireless requirements that must be defined before conducting a wireless site survey or developing an enterprise Wi-Fi design.

A successful wireless network begins with clearly defined requirements. The information collected during this phase directly influences the survey methodology, AP placement, RF design, channel planning, capacity planning, security architecture, and validation criteria.

---

## Objectives

The objectives of this phase are to:

* Understand business and operational requirements
* Identify users, devices, applications, and locations
* Define coverage and performance expectations
* Determine capacity and client-density requirements
* Identify security and authentication requirements
* Understand regulatory and compliance requirements
* Define survey scope and methodology
* Establish measurable design and acceptance criteria

---

## Requirements and Planning Process

```text
Business Requirements
        │
        ▼
User and Device Requirements
        │
        ▼
Application Requirements
        │
        ▼
Coverage and Capacity Requirements
        │
        ▼
Security Requirements
        │
        ▼
Survey Planning
        │
        ▼
Design Acceptance Criteria
```

---

## Directory Contents

| File                                   | Description                                                                  |
| -------------------------------------- | ---------------------------------------------------------------------------- |
| `client-requirements-questionnaire.md` | Questions to collect business and technical requirements from the customer   |
| `application-requirements.md`          | Requirements for voice, video, collaboration, IoT, and business applications |
| `survey-planning-checklist.md`         | Checklist for preparing and executing a wireless site survey                 |
| `wireless-design-requirements.md`      | General technical requirements for the wireless network design               |
| `capacity-and-density-requirements.md` | User density, client count, throughput, and capacity requirements            |
| `coverage-requirements.md`             | Coverage, signal strength, SNR, and roaming requirements                     |
| `security-requirements.md`             | Authentication, encryption, segmentation, and security requirements          |
| `acceptance-criteria.md`               | Measurable criteria used to validate the completed wireless network          |

---

## Key Requirement Categories

### 1. Business Requirements

Identify:

* Business locations and buildings
* Business-critical areas
* Operating hours
* Business-critical applications
* Required network availability
* Growth expectations
* Budget and project constraints

---

### 2. User Requirements

Identify:

* Number of users
* User types
* User mobility requirements
* BYOD requirements
* Guest access requirements
* Remote or temporary users
* Special user groups

Example:

```text
Employees
Contractors
Visitors
Executives
Warehouse Staff
Production Users
IoT Devices
Voice Users
```

---

### 3. Device Requirements

Document:

* Number of wireless clients
* Client types
* Wi-Fi standards supported
* 2.4 GHz requirements
* 5 GHz requirements
* 6 GHz requirements
* Legacy client requirements
* IoT devices
* Barcode scanners
* Wireless printers
* Medical or industrial devices

---

### 4. Application Requirements

Identify applications that will use the wireless network.

Examples:

* Microsoft Teams
* Voice over Wi-Fi
* Video conferencing
* Cloud applications
* ERP applications
* Warehouse management systems
* Barcode scanning
* Location services
* IoT applications
* Industrial automation

Each critical application should be evaluated for:

* Bandwidth
* Latency
* Jitter
* Packet loss
* Roaming requirements
* Availability requirements

---

### 5. Coverage Requirements

Define the required coverage area and minimum performance requirements.

Typical parameters include:

| Requirement     | Example               |
| --------------- | --------------------- |
| Coverage        | -67 dBm               |
| Voice coverage  | -67 dBm or better     |
| Data coverage   | -67 to -70 dBm        |
| SNR             | 25 dB or higher       |
| Roaming overlap | 15–20%                |
| Packet loss     | Application dependent |

The final values must be agreed with the customer and aligned with application requirements.

---

### 6. Capacity and Density Requirements

Capacity planning should consider:

```text
Number of Users
        +
Number of Devices
        +
Application Traffic
        +
Peak Usage
        +
Future Growth
        =
Required Wireless Capacity
```

Important information includes:

* Average clients per AP
* Peak client count
* High-density areas
* Expected concurrent users
* Expected traffic per user
* Future growth
* Special events or peak periods

---

### 7. Security Requirements

Define:

* SSID architecture
* WPA2/WPA3 requirements
* 802.1X authentication
* RADIUS requirements
* Certificate-based authentication
* Guest access
* BYOD access
* Device onboarding
* Network segmentation
* Role-based access control
* NAC integration

Example technologies:

```text
802.1X
RADIUS
Cisco ISE
Aruba ClearPass
WPA2-Enterprise
WPA3-Enterprise
EAP-TLS
PEAP
MAC Authentication Bypass
Guest Captive Portal
```

---

### 8. Survey Planning

Before beginning the survey, define:

* Survey type
* Survey scope
* Building floor plans
* Areas to be surveyed
* Operating hours
* Survey equipment
* Survey software
* AP models
* Antenna types
* Mounting constraints
* Access requirements
* Safety requirements

Possible survey types:

```text
Predictive Survey
Passive Survey
Active Survey
AP-on-a-Stick Survey
Spectrum Analysis
Post-Deployment Validation Survey
```

---

## Recommended Requirement Workflow

### Step 1 - Understand the Environment

Collect:

* Building plans
* Floor plans
* Construction materials
* Ceiling height
* Wall types
* Existing network topology
* Existing AP locations

---

### Step 2 - Understand the Users and Devices

Document:

* Number of users
* Number of devices
* Device types
* Mobility requirements
* High-density areas

---

### Step 3 - Understand the Applications

Identify:

* Business-critical applications
* Real-time applications
* Cloud applications
* Voice and video requirements
* IoT applications

---

### Step 4 - Define Technical Targets

Establish:

* Minimum RSSI
* Minimum SNR
* Channel width
* Capacity targets
* Roaming requirements
* Availability requirements

---

### Step 5 - Plan the Survey

Define:

* Survey methodology
* Survey equipment
* Survey areas
* AP-on-a-Stick locations
* Required documentation

---

### Step 6 - Define Acceptance Criteria

The wireless design should have measurable validation criteria.

Example:

```text
Coverage:
Minimum RSSI: -67 dBm

Signal Quality:
Minimum SNR: 25 dB

Roaming:
Seamless roaming for voice clients

Capacity:
Maximum average clients per AP defined by design

Availability:
Wireless service must meet agreed SLA

Security:
All corporate clients must authenticate using 802.1X
```

---

## Requirements Traceability

All requirements should be traceable throughout the project.

```text
Requirement
    │
    ▼
Survey
    │
    ▼
RF Design
    │
    ▼
AP Placement
    │
    ▼
Implementation
    │
    ▼
Validation
    │
    ▼
Acceptance
```

This ensures that the final wireless network meets the original business and technical requirements.

---

## Best Practices

* Do not start a wireless survey without understanding the requirements.
* Do not design only for coverage; design for capacity and application performance.
* Always identify critical applications.
* Consider future growth during the initial design.
* Document high-density areas separately.
* Validate requirements with the customer.
* Use measurable acceptance criteria.
* Maintain traceability between requirements and final design.
* Document assumptions and design constraints.
* Review requirements whenever the project scope changes.

---

## Related Directories

```text
01-Requirements-and-Planning/
        │
        ├── 02-Site-Survey/
        ├── 03-RF-Design/
        ├── 04-AP-Placement/
        ├── 05-Wireless-Architecture/
        └── 07-Validation-and-Testing/
```

---

## Requirement Status

| Category                 | Status        |
| ------------------------ | ------------- |
| Business Requirements    | ☐ Not Started |
| User Requirements        | ☐ Not Started |
| Device Requirements      | ☐ Not Started |
| Application Requirements | ☐ Not Started |
| Coverage Requirements    | ☐ Not Started |
| Capacity Requirements    | ☐ Not Started |
| Security Requirements    | ☐ Not Started |
| Survey Planning          | ☐ Not Started |
| Acceptance Criteria      | ☐ Not Started |

---

## Document Control

| Version | Date       | Author                   | Description     |
| ------- | ---------- | ------------------------ | --------------- |
| 1.0     | YYYY-MM-DD | Network Engineering Team | Initial version |
