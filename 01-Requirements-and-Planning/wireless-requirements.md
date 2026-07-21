# Wireless Requirements Document

## 1. Document Information

| Item                    | Details |
| ----------------------- | ------- |
| Project Name            |         |
| Customer / Organization |         |
| Site / Location         |         |
| Building / Campus       |         |
| Number of Floors        |         |
| Document Owner          |         |
| Version                 |         |
| Date                    |         |

---

## 2. Project Overview

Describe the purpose of the wireless deployment or upgrade.

Example:

> The objective of this project is to design and deploy a reliable, secure, scalable, and high-performing enterprise wireless network that supports business-critical applications, users, IoT devices, voice, mobility, and future growth.

---

## 3. Business Requirements

Document the business objectives of the wireless network.

### Requirements

* [ ] Reliable wireless connectivity
* [ ] High availability
* [ ] Improved wireless coverage
* [ ] Increased capacity
* [ ] Support for business-critical applications
* [ ] Support for mobility
* [ ] Support for IoT devices
* [ ] Guest wireless access
* [ ] Future scalability

### Business Requirements

| Requirement | Description | Priority            |
| ----------- | ----------- | ------------------- |
|             |             | High / Medium / Low |
|             |             | High / Medium / Low |
|             |             | High / Medium / Low |

---

## 4. Coverage Requirements

Identify the areas requiring wireless coverage.

| Area            | Required Coverage | Priority |
| --------------- | ----------------- | -------- |
| Office          | Yes / No          |          |
| Meeting Rooms   | Yes / No          |          |
| Corridors       | Yes / No          |          |
| Warehouse       | Yes / No          |          |
| Production Area | Yes / No          |          |
| Outdoor Area    | Yes / No          |          |
| Parking Area    | Yes / No          |          |

---

## 5. Coverage Design Targets

Define the minimum acceptable wireless performance.

| Metric                      | Target |
| --------------------------- | ------ |
| Minimum RSSI                |        |
| Minimum SNR                 |        |
| Maximum Noise Floor         |        |
| Maximum Channel Utilization |        |
| Minimum Data Rate           |        |
| Maximum Packet Loss         |        |
| Maximum Latency             |        |

Example design targets:

```text
RSSI:              -67 dBm or better
SNR:                25 dB or better
Noise Floor:       -85 dBm or lower
Channel Utilization: < 50%
Packet Loss:        < 1%
```

> Design targets must be validated against the application and business requirements.

---

## 6. Capacity Requirements

Document the expected number of users and devices.

| Item                    | Quantity |
| ----------------------- | -------: |
| Total Users             |          |
| Total Wireless Devices  |          |
| Peak Concurrent Devices |          |
| Voice Devices           |          |
| IoT Devices             |          |
| Guest Devices           |          |
| High-Bandwidth Devices  |          |

---

## 7. Application Requirements

| Application    | Users / Devices | Bandwidth | Latency | Roaming               |
| -------------- | --------------: | --------- | ------- | --------------------- |
| Voice          |                 |           |         | Required              |
| Video          |                 |           |         | Required              |
| Data           |                 |           |         | Optional              |
| IoT            |                 |           |         | Application dependent |
| Guest Internet |                 |           |         | Optional              |

---

## 8. Wireless Security Requirements

Document the required security model.

### Authentication

* [ ] WPA2-Enterprise
* [ ] WPA3-Enterprise
* [ ] 802.1X
* [ ] Certificate Authentication
* [ ] PSK
* [ ] MPSK
* [ ] MAC Authentication Bypass

### Identity and Access Control

* [ ] Dynamic VLAN Assignment
* [ ] Dynamic Role Assignment
* [ ] Network Access Control
* [ ] Guest Authentication
* [ ] Device Profiling
* [ ] IoT Segmentation

### Security Platforms

* [ ] Aruba ClearPass
* [ ] Cisco ISE
* [ ] Microsoft NPS
* [ ] Other: __________

---

## 9. SSID Requirements

| SSID      | Purpose | Authentication | VLAN / Role |
| --------- | ------- | -------------- | ----------- |
| Corporate |         |                |             |
| Guest     |         |                |             |
| IoT       |         |                |             |
| Voice     |         |                |             |

### SSID Design Principles

* Minimize unnecessary SSIDs
* Avoid excessive broadcast overhead
* Use appropriate authentication
* Apply role-based access control
* Segment different device types
* Use appropriate QoS policies

---

## 10. Mobility and Roaming Requirements

Document whether fast roaming is required.

* [ ] 802.11k
* [ ] 802.11v
* [ ] 802.11r
* [ ] Fast roaming
* [ ] Voice roaming
* [ ] Seamless application mobility

### Roaming Applications

* Voice
* Video
* Warehouse scanners
* Healthcare devices
* Industrial mobility
* Real-time applications

---

## 11. Regulatory and RF Requirements

Document the regulatory domain:

```text
Country / Region:
Regulatory Domain:
Supported Bands:
2.4 GHz: Yes / No
5 GHz:   Yes / No
6 GHz:   Yes / No
DFS Allowed: Yes / No
```

---

## 12. Existing Infrastructure

Document the current environment.

| Component                   | Details |
| --------------------------- | ------- |
| Wireless Platform           |         |
| AP Model                    |         |
| Controller / Cloud Platform |         |
| Switch Platform             |         |
| PoE Availability            |         |
| Authentication Platform     |         |
| Existing SSIDs              |         |
| Existing RF Issues          |         |

---

## 13. Future Growth

Consider expected growth over the next:

* 1 year
* 3 years
* 5 years

Consider:

* Additional users
* Additional devices
* New applications
* IoT expansion
* Wi-Fi 6E / Wi-Fi 7 adoption
* Increased bandwidth requirements

---

## 14. Final Requirements Summary

Before beginning the wireless design, confirm:

* [ ] Coverage requirements approved
* [ ] Capacity requirements approved
* [ ] Application requirements documented
* [ ] Security requirements approved
* [ ] Roaming requirements documented
* [ ] Regulatory requirements confirmed
* [ ] Existing infrastructure documented
* [ ] Future growth considered

---

## 15. Approval

| Role               | Name | Approval | Date |
| ------------------ | ---- | -------- | ---- |
| Business Owner     |      |          |      |
| IT Owner           |      |          |      |
| Network Architect  |      |          |      |
| Security Architect |      |          |      |

---

> **Design Principle:** Wireless design requirements should be driven by business applications, client behavior, performance expectations, security requirements, and future growth—not only by coverage.

