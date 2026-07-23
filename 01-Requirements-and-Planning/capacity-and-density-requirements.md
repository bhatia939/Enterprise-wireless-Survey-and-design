# Capacity and Density Requirements

This document defines the requirements for planning wireless network capacity and client density in enterprise Wi-Fi environments.

A wireless network must be designed not only to provide coverage, but also to support the expected number of users, devices, applications, traffic volumes, and future growth.

---

## 1. Purpose

The purpose of this document is to define requirements for:

* Wireless client capacity
* User density
* Device density
* Application traffic
* Airtime utilization
* High-density environments
* Peak usage
* Future growth
* AP capacity
* Radio capacity
* Capacity validation

---

## 2. Capacity Design Principle

Wireless capacity is primarily an **airtime resource**.

The capacity of a wireless network depends on:

```text
Number of Clients
        +
Traffic Demand
        +
Application Requirements
        +
Available Airtime
        +
RF Conditions
        +
Channel Configuration
        =
Wireless Capacity
```

A design with strong signal strength can still provide poor performance if the available airtime is overloaded.

---

## 3. Capacity Planning Objectives

The wireless design should:

* Support the expected number of concurrent clients
* Support application traffic requirements
* Maintain acceptable airtime utilization
* Support peak usage periods
* Provide sufficient capacity for growth
* Avoid excessive client concentration
* Support high-density areas
* Maintain application performance

---

## 4. User and Device Inventory

The following information should be collected.

### User Information

* [ ] Total number of users
* [ ] Average concurrent users
* [ ] Peak concurrent users
* [ ] Mobile users
* [ ] Stationary users
* [ ] Guest users
* [ ] Contractors
* [ ] Temporary users
* [ ] Expected user growth

### Device Information

* [ ] Laptops
* [ ] Smartphones
* [ ] Tablets
* [ ] Voice handsets
* [ ] Barcode scanners
* [ ] Printers
* [ ] IoT devices
* [ ] Industrial devices
* [ ] Cameras
* [ ] Sensors
* [ ] Special-purpose wireless devices

Example:

```text
Users
  │
  ├── 500 Employees
  ├── 100 Guests
  └── 50 Contractors

Devices
  │
  ├── 650 Laptops
  ├── 500 Smartphones
  ├── 100 IoT Devices
  └── 50 Voice Devices
```

---

## 5. Concurrent Client Calculation

Total registered devices are not always connected at the same time.

The design should distinguish between:

```text
Total Devices
        ↓
Expected Active Devices
        ↓
Peak Concurrent Devices
        ↓
Peak Traffic Demand
```

Example:

```text
1,000 Registered Devices
        ↓
700 Regularly Active Devices
        ↓
500 Concurrent Devices
        ↓
Peak Usage Period
```

The wireless design should be based on realistic peak concurrency rather than only the total number of registered devices.

---

## 6. Client Density Categories

Different areas should be classified according to client density.

### Low Density

Examples:

* Small offices
* Storage areas
* Low-use corridors

Characteristics:

* Few clients
* Low traffic
* Limited concurrent usage

---

### Medium Density

Examples:

* Standard offices
* Meeting rooms
* Common areas

Characteristics:

* Moderate client count
* Normal business applications
* Regular concurrent usage

---

### High Density

Examples:

* Conference rooms
* Classrooms
* Auditoriums
* Cafeterias
* Training centers
* Event areas

Characteristics:

* High client concentration
* High concurrent usage
* High traffic demand
* Increased contention

---

### Very High Density

Examples:

* Stadiums
* Large auditoriums
* Exhibition halls
* Large conference venues

These environments require detailed capacity engineering and often require specialized RF design.

---

## 7. Application Traffic Requirements

Each application should be classified according to its traffic requirements.

| Application Type   | Traffic Profile | Sensitivity           |
| ------------------ | --------------- | --------------------- |
| Web Browsing       | Variable        | Low                   |
| Email              | Low to Medium   | Low                   |
| Cloud Applications | Variable        | Medium                |
| Voice              | Low             | High                  |
| Video Conferencing | Medium to High  | High                  |
| Video Streaming    | High            | Medium                |
| File Transfer      | High            | Medium                |
| IoT                | Low             | Application dependent |

For critical applications, document:

* Bandwidth requirement
* Latency requirement
* Jitter requirement
* Packet-loss tolerance
* Concurrent users
* Peak usage

---

## 8. Application Capacity Model

The capacity requirement should be calculated based on concurrent usage.

Example:

```text
Concurrent Users
        ×
Average Application Throughput
        =
Required Aggregate Throughput
```

Example:

```text
50 Concurrent Users
        ×
2 Mbps per User
        =
100 Mbps Aggregate Demand
```

The design must also consider:

* Protocol overhead
* Retransmissions
* RF conditions
* Airtime efficiency
* Peak demand

Theoretical PHY rate must not be treated as actual application throughput.

---

## 9. Airtime Utilization

Wireless networks share airtime between clients.

Airtime is consumed by:

* Data transmission
* Management frames
* Control frames
* Retransmissions
* Interference
* Low-rate clients

A slow client can consume significantly more airtime than a fast client transmitting the same amount of data.

The design should therefore consider:

```text
Airtime Demand
        +
Client Data Rates
        +
Retransmissions
        +
Protocol Overhead
```

---

## 10. Channel Utilization

Channel utilization should be monitored and validated.

High utilization can result from:

* Too many clients
* High traffic volume
* Excessive AP density
* Co-channel interference
* Non-Wi-Fi interference
* Excessive channel width

The design should define acceptable channel utilization thresholds based on:

* Application requirements
* Client density
* Traffic profiles
* RF environment

---

## 11. AP Capacity Planning

AP capacity depends on:

* AP hardware
* Radio capabilities
* Spatial streams
* Channel width
* Client capabilities
* Airtime availability
* Application traffic
* RF environment

The maximum theoretical client count advertised by a vendor should not automatically be used as the design target.

The design should define:

```text
Recommended Clients per Radio
        +
Expected Traffic per Client
        +
Peak Airtime Utilization
```

---

## 12. Client Distribution

Clients should be distributed across available APs and channels where possible.

The design should avoid:

```text
AP 1: 80 Clients
AP 2: 10 Clients
AP 3: 8 Clients
```

Where possible, the design should achieve a more balanced distribution.

However, client distribution is ultimately influenced by:

* Client roaming decisions
* Client transmit power
* AP power levels
* RF conditions
* Client drivers

The network should therefore be designed to encourage, but not assume, perfect client distribution.

---

## 13. High-Density Area Requirements

For each high-density area, document:

| Requirement               | Value |
| ------------------------- | ----- |
| Area                      |       |
| Expected users            |       |
| Expected devices per user |       |
| Peak concurrent clients   |       |
| Applications              |       |
| Peak traffic              |       |
| Required coverage         |       |
| Required capacity         |       |
| Future growth             |       |

Example:

```text
Area:
Conference Room

Users:
100

Devices per User:
2

Expected Devices:
200

Peak Concurrent Devices:
180

Applications:
Teams, Web, Cloud Applications

Design:
Capacity-focused RF design required
```

---

## 14. High-Density Design Principles

High-density designs may require:

* More APs
* Lower transmit power
* Smaller cells
* Narrower channel widths
* Greater channel reuse
* Increased 5 GHz usage
* Increased 6 GHz usage
* Careful client distribution

Important:

> Adding more APs without a proper channel and power plan can reduce performance because of increased co-channel interference.

---

## 15. 2.4 GHz Capacity Requirements

The 2.4 GHz band has limited channel availability.

Capacity planning must consider:

* Limited non-overlapping channels
* High interference
* Legacy devices
* IoT requirements

Recommended approach:

```text
2.4 GHz
    ↓
Use only where required
    ↓
20 MHz Channels
    ↓
Limit Client Density
```

---

## 16. 5 GHz Capacity Requirements

The 5 GHz band generally provides more capacity than 2.4 GHz.

Consider:

* Available channels
* DFS channels
* Channel width
* Client compatibility
* Transmit power
* Channel reuse

The design should avoid automatically selecting the widest channel width.

---

## 17. 6 GHz Capacity Requirements

The 6 GHz band can provide additional capacity through additional spectrum.

Consider:

* Compatible clients
* AP capabilities
* Regulatory requirements
* Channel width
* Power levels
* Security requirements

6 GHz should be included where it provides a measurable capacity or performance benefit.

---

## 18. Voice Capacity Requirements

Voice applications typically consume relatively little bandwidth but require consistent airtime and low latency.

Capacity planning should consider:

* Number of concurrent calls
* Codec
* Roaming
* Packet loss
* Jitter
* Latency
* Airtime utilization

The design must ensure that voice clients are not placed in congested RF environments.

---

## 19. Video and Collaboration Capacity

Video conferencing may create significant traffic demand.

Consider:

* Number of concurrent video sessions
* Video resolution
* Upload traffic
* Download traffic
* Peak meeting times
* Application behavior

High-density meeting areas should be evaluated separately from standard office areas.

---

## 20. IoT and Specialized Device Capacity

IoT devices may have different traffic characteristics.

Consider:

* Number of devices
* Packet size
* Transmission frequency
* Battery limitations
* Required data rate
* Mobility
* Security requirements

Some IoT deployments may require:

* Dedicated SSIDs
* Dedicated VLANs
* Dedicated APs
* Specialized radio technologies

---

## 21. Growth and Scalability

Capacity planning must include future growth.

Consider:

* User growth
* Device growth
* New applications
* Increased cloud usage
* Additional business units
* Building expansion

Example:

```text
Current:
500 Concurrent Clients

Year 1:
650 Concurrent Clients

Year 3:
900 Concurrent Clients
```

The design should provide a reasonable growth margin.

---

## 22. Capacity Planning Data Collection

The following data should be collected where available:

* Current client count
* Peak client count
* Average client count
* AP utilization
* Channel utilization
* Application traffic
* Peak traffic periods
* Client data rates
* Retransmission rates
* Noise levels
* Existing performance issues

Data sources may include:

* Wireless management platform
* Network monitoring system
* Application monitoring
* Client telemetry
* Existing survey data

---

## 23. Capacity Validation

Capacity should be validated after implementation.

Validation may include:

* Concurrent client testing
* Throughput testing
* Application testing
* Channel utilization analysis
* Client distribution analysis
* Load testing
* Voice testing
* Video conferencing validation

The validation should be performed during representative usage periods where possible.

---

## 24. Capacity Acceptance Criteria

The wireless design should meet the approved capacity requirements.

Example:

```text
Client Capacity:
Supports expected concurrent clients.

Application Capacity:
Supports expected application traffic.

Airtime:
Remains within the approved utilization target.

Client Distribution:
No unacceptable client concentration.

High-Density Areas:
Meet defined performance requirements.

Growth:
Provides sufficient capacity for planned growth.
```

---

## 25. Capacity Exceptions

Any capacity limitation must be documented.

For each exception, record:

* Location
* Expected client count
* Actual capacity
* Performance impact
* Root cause
* Recommended solution
* Business risk
* Customer approval

Example:

```text
Location:
Training Room

Issue:
Peak client density exceeds planned capacity.

Impact:
Reduced throughput during training sessions.

Recommendation:
Add capacity-focused AP and optimize channel reuse.

Status:
Design change required.
```

---

## 26. Capacity Planning Workflow

```text
Identify Users
        │
        ▼
Identify Devices
        │
        ▼
Identify Applications
        │
        ▼
Calculate Peak Concurrency
        │
        ▼
Estimate Traffic Demand
        │
        ▼
Analyze Airtime Requirements
        │
        ▼
Design AP Density
        │
        ▼
Design Channel Reuse
        │
        ▼
Validate Capacity
        │
        ▼
Document Results
```

---

## 27. Capacity Planning Checklist

* [ ] Total users documented
* [ ] Total devices documented
* [ ] Concurrent users identified
* [ ] Peak usage identified
* [ ] Application traffic documented
* [ ] High-density areas identified
* [ ] Client density calculated
* [ ] AP capacity evaluated
* [ ] Airtime requirements evaluated
* [ ] Channel utilization requirements defined
* [ ] 2.4 GHz requirements defined
* [ ] 5 GHz requirements defined
* [ ] 6 GHz requirements defined
* [ ] Voice capacity requirements defined
* [ ] Video capacity requirements defined
* [ ] IoT capacity requirements defined
* [ ] Growth requirements defined
* [ ] Capacity validation plan defined
* [ ] Acceptance criteria approved

---

## Document Control

| Version | Date       | Author                   | Description     |
| ------- | ---------- | ------------------------ | --------------- |
| 1.0     | YYYY-MM-DD | Network Engineering Team | Initial version |

