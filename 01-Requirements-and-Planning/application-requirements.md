# Application Requirements

Application requirements define how wireless network performance will be evaluated for the applications used by the organization.

Wireless design should be based on application behavior and performance requirements—not only on signal coverage.

---

## 1. Application Inventory

Document all applications that will use the wireless network.

| Application | Category | Users / Devices | Criticality         |
| ----------- | -------- | --------------: | ------------------- |
|             |          |                 | High / Medium / Low |
|             |          |                 | High / Medium / Low |
|             |          |                 | High / Medium / Low |

---

## 2. Application Categories

### 💻 Data Applications

Examples:

* Web browsing
* Email
* File sharing
* ERP
* CRM
* Database applications
* Cloud applications

Typical requirements:

```text
Bandwidth:       Low to High
Latency:         Low to Medium
Packet Loss:     Low
Roaming:         Application dependent
```

---

### 📞 Voice over Wi-Fi

Examples:

* Wi-Fi handsets
* Softphones
* Mobile voice applications

Important requirements:

| Metric      | Typical Target    |
| ----------- | ----------------- |
| RSSI        | -67 dBm or better |
| SNR         | 25 dB or better   |
| Packet Loss | < 1%              |
| Latency     | < 100 ms          |
| Jitter      | < 30 ms           |
| Roaming     | Required          |

Voice applications require consistent coverage and reliable roaming.

---

### 🎥 Video Applications

Examples:

* Video conferencing
* Microsoft Teams
* Zoom
* Webex
* Streaming

Important considerations:

* High bandwidth
* Low packet loss
* Low latency
* Stable RF coverage
* Sufficient capacity

---

### 🏭 Warehouse Applications

Examples:

* Barcode scanners
* Handheld terminals
* Warehouse management systems
* Automated guided vehicles

Important considerations:

* Continuous coverage
* Fast roaming
* Low latency
* High device mobility
* Metal rack attenuation
* High client density

---

### 🏥 Healthcare Applications

Examples:

* Medical devices
* Patient monitoring
* Voice communication
* Clinical applications

Requirements may include:

* High availability
* Secure authentication
* Reliable roaming
* Low packet loss
* Application-specific QoS

---

### 🏷️ IoT Applications

Examples:

* Sensors
* Building management systems
* Smart devices
* Industrial monitoring
* Environmental sensors

Consider:

* Device density
* Battery life
* Low bandwidth
* Security
* Authentication
* Network segmentation

---

## 3. Application Performance Requirements

| Application | Bandwidth | Latency               | Jitter    | Packet Loss           | Roaming  |
| ----------- | --------- | --------------------- | --------- | --------------------- | -------- |
| Voice       | Low       | Low                   | Critical  | Very Low              | Required |
| Video       | High      | Low                   | Important | Low                   | Required |
| Data        | Medium    | Medium                | Normal    | Low                   | Optional |
| IoT         | Low       | Application dependent | Normal    | Application dependent | Optional |
| Warehouse   | Medium    | Low                   | Important | Low                   | Required |

> These values are general planning guidelines. Actual requirements must be confirmed with the application owner and vendor documentation.

---

## 4. Application Criticality

Classify each application.

### Critical

Failure directly impacts business operations.

Examples:

* Production systems
* Healthcare applications
* Warehouse operations
* Point-of-Sale systems

### Important

Performance degradation impacts productivity.

Examples:

* Video conferencing
* ERP
* CRM

### Standard

Temporary disruption has limited business impact.

Examples:

* Guest Internet
* General web browsing

---

## 5. Bandwidth Requirements

Document the expected bandwidth.

| Application | Average Bandwidth | Peak Bandwidth | Total Users | Total Capacity |
| ----------- | ----------------: | -------------: | ----------: | -------------: |
|             |                   |                |             |                |
|             |                   |                |             |                |
|             |                   |                |             |                |

### Capacity Calculation

```text
Total Required Capacity =
Number of Concurrent Users × Average Bandwidth per User
```

Example:

```text
100 users × 5 Mbps
= 500 Mbps required capacity
```

---

## 6. Latency Requirements

Document latency-sensitive applications.

| Application        | Maximum Acceptable Latency |
| ------------------ | -------------------------: |
| Voice              |                            |
| Video              |                            |
| Industrial Control |                            |
| Data               |                            |
| IoT                |                            |

---

## 7. Roaming Requirements

Determine whether the application requires seamless mobility.

| Application | Mobility | Roaming Required      | Fast Roaming          |
| ----------- | -------- | --------------------- | --------------------- |
| Voice       | High     | Yes                   | Yes                   |
| Warehouse   | High     | Yes                   | Yes                   |
| Video       | Medium   | Yes                   | Application dependent |
| Office Data | Low      | Optional              | Optional              |
| IoT         | Low      | Application dependent | Application dependent |

Potential WLAN features:

* 802.11k
* 802.11v
* 802.11r
* Fast BSS Transition
* Client steering

---

## 8. Quality of Service Requirements

Identify applications requiring QoS.

Typical traffic categories:

```text
Voice
  │
  ▼
Highest Priority

Video
  │
  ▼
High Priority

Business Data
  │
  ▼
Normal Priority

Guest / Background Traffic
  │
  ▼
Lower Priority
```

Consider:

* DSCP marking
* WMM
* 802.11e
* Application classification
* Traffic shaping
* Bandwidth limits

---

## 9. Application Security Requirements

Document security requirements for each application.

| Application | Authentication    | Encryption | Segmentation |
| ----------- | ----------------- | ---------- | ------------ |
| Corporate   | 802.1X            | WPA2/WPA3  | Required     |
| Guest       | Captive Portal    | WPA2/WPA3  | Required     |
| IoT         | PSK / Certificate | WPA2/WPA3  | Required     |
| Voice       | 802.1X / PSK      | WPA2/WPA3  | Required     |

---

## 10. Application Dependency Mapping

Document dependencies.

```text
Wireless Client
      │
      ▼
      AP
      │
      ▼
Wireless Controller / Cloud
      │
      ▼
      LAN
      │
      ▼
Firewall / WAN
      │
      ▼
Application / Cloud Service
```

Identify dependencies such as:

* DHCP
* DNS
* RADIUS
* Active Directory
* PKI
* Internet
* WAN
* Data Center
* Cloud Services

---

## 11. Application Testing Requirements

Define how each application will be validated after deployment.

| Application | Test Method         | Success Criteria           |
| ----------- | ------------------- | -------------------------- |
| Voice       | Call test           | Clear voice / no drops     |
| Video       | Video call          | No significant degradation |
| Data        | Throughput test     | Meets requirement          |
| Warehouse   | Mobility test       | No application disconnect  |
| IoT         | Device connectivity | Stable connectivity        |

---

## 12. Application Requirements Summary

### Critical Applications

1. ---
2. ---
3. ---

### Most Bandwidth-Intensive Applications

1. ---
2. ---
3. ---

### Most Latency-Sensitive Applications

1. ---
2. ---
3. ---

### Applications Requiring Roaming

1. ---
2. ---
3. ---

---

## 13. Final Application Validation

Before finalizing the wireless design:

* [ ] All applications identified
* [ ] Application owners consulted
* [ ] Bandwidth requirements documented
* [ ] Latency requirements documented
* [ ] Roaming requirements documented
* [ ] QoS requirements documented
* [ ] Security requirements documented
* [ ] Application testing defined
* [ ] Success criteria approved

---

> **Design Principle:** The wireless network should be designed to meet the performance requirements of the most demanding business-critical applications.

