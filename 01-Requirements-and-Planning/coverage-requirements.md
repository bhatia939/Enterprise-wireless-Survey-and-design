# Wireless Coverage Requirements

This document defines the coverage requirements for an enterprise wireless network. It establishes the minimum RF performance required to support users, applications, devices, voice services, roaming, and business-critical wireless operations.

Coverage requirements must be defined before completing the final RF design and AP placement.

---

## 1. Purpose

The purpose of this document is to define:

* Minimum received signal strength
* Minimum signal-to-noise ratio
* Required coverage areas
* Roaming coverage requirements
* Voice and real-time application requirements
* Coverage overlap requirements
* 2.4 GHz, 5 GHz, and 6 GHz requirements
* Outdoor coverage requirements
* Validation and acceptance criteria

---

## 2. Coverage Design Principles

Wireless coverage should not be designed only to provide a visible Wi-Fi signal.

A successful wireless design must provide:

```text
Required Coverage
        +
Required Signal Quality
        +
Required Capacity
        +
Required Roaming
        +
Required Application Performance
        =
Successful Wireless Design
```

The required RF targets should be based on the most demanding application and device requirements.

---

## 3. Coverage Areas

The following areas should be identified and classified.

### Standard Office Areas

Examples:

* Open offices
* Private offices
* Corridors
* Reception areas
* Common areas

Typical requirements:

* Reliable data connectivity
* Business application access
* Email and cloud application access
* Web browsing
* Collaboration applications

---

### High-Density Areas

Examples:

* Conference rooms
* Training rooms
* Classrooms
* Auditoriums
* Cafeterias
* Event spaces

These areas require separate capacity planning in addition to coverage planning.

Requirements should include:

* Number of users
* Number of devices
* Concurrent clients
* Application usage
* Peak traffic
* Expected growth

---

### Voice and Real-Time Areas

Examples:

* Offices
* Warehouses
* Production areas
* Hospitals
* Campus environments

These areas require:

* Consistent signal strength
* Sufficient SNR
* Adequate cell overlap
* Low packet loss
* Low latency
* Reliable roaming

---

### Outdoor Areas

Examples:

* Parking areas
* Loading docks
* Courtyards
* Campus walkways
* Outdoor work areas

Outdoor coverage must consider:

* AP mounting locations
* Weather protection
* Antenna patterns
* Cable distances
* Lightning protection
* Environmental conditions

---

## 4. RSSI Requirements

Received Signal Strength Indicator (RSSI) represents the strength of the wireless signal received by a client.

RSSI is measured in dBm.

The value is negative. A value closer to zero represents a stronger signal.

Example:

```text
-45 dBm  = Excellent
-60 dBm  = Very Good
-67 dBm  = Common enterprise design target
-70 dBm  = Acceptable for some data applications
-80 dBm  = Weak
```

### Recommended Design Targets

| Use Case                      | Recommended Minimum RSSI               |
| ----------------------------- | -------------------------------------- |
| General data                  | -67 to -70 dBm                         |
| Voice over Wi-Fi              | -67 dBm                                |
| Video applications            | -67 dBm                                |
| High-performance applications | -65 dBm or better                      |
| Location services             | Based on location accuracy requirement |
| IoT                           | Based on device requirements           |
| Industrial applications       | Application dependent                  |

The final target must be selected based on actual business and application requirements.

---

## 5. Signal-to-Noise Ratio Requirements

Signal-to-Noise Ratio (SNR) represents the difference between the received signal and the background noise.

Higher SNR generally provides better wireless performance.

### Recommended Targets

| Application                   | Minimum SNR           |
| ----------------------------- | --------------------- |
| Basic data                    | 20 dB                 |
| Enterprise data               | 25 dB                 |
| Voice                         | 25 dB                 |
| High-performance applications | 25–30 dB              |
| Critical applications         | Application dependent |

Example:

```text
Signal: -67 dBm
Noise:  -92 dBm

SNR = 25 dB
```

A strong RSSI with a high noise floor may still result in poor wireless performance.

---

## 6. Noise Floor Requirements

The noise floor represents the background RF energy detected by the wireless receiver.

Recommended targets:

```text
Excellent:  -95 dBm or lower
Good:       -92 dBm or lower
Acceptable: -85 dBm or lower
```

The actual acceptable noise floor depends on the environment and application.

A high noise floor can cause:

* Reduced data rates
* Increased retransmissions
* Poor roaming
* Increased latency
* Reduced capacity

---

## 7. Channel Utilization Requirements

Channel utilization should be evaluated during the survey.

High channel utilization may indicate:

* Too many clients
* Excessive AP density
* Non-Wi-Fi interference
* Excessive channel width
* High traffic volume

Recommended planning approach:

```text
Low Utilization:
Preferred

Moderate Utilization:
Acceptable depending on capacity requirements

High Utilization:
Requires investigation and capacity planning
```

The exact threshold should be defined based on the environment and expected traffic.

---

## 8. Coverage Overlap Requirements

Wireless cells should provide sufficient overlap to support client roaming.

Coverage overlap should be based on:

* Client capabilities
* Application requirements
* Roaming protocol
* Voice requirements
* AP density
* Cell size

For voice and real-time applications, the client should be able to discover the next AP before the current connection becomes unusable.

Example design principle:

```text
AP 1 Coverage
        ◄──────►
      Overlap
        ◄──────►
AP 2 Coverage
```

Avoid excessive overlap because it can increase:

* Co-channel interference
* Contention
* Channel utilization
* Reduced capacity

---

## 9. Roaming Requirements

Roaming requirements must be defined for mobile clients.

The design should consider:

* Client roaming behavior
* 802.11k
* 802.11v
* 802.11r
* Fast transition requirements
* Application sensitivity
* Client driver capabilities

### Voice Roaming

Voice clients typically require:

* Consistent RF coverage
* Adequate overlap
* Low packet loss
* Low latency
* Fast roaming
* Stable authentication

The roaming design must be validated with the actual client devices used in the environment.

---

## 10. Frequency Band Requirements

### 2.4 GHz

The 2.4 GHz band provides:

* Greater propagation range
* Better wall penetration
* Support for legacy devices
* Support for some IoT devices

However, it has:

* Limited available channels
* Greater interference
* Higher congestion

Recommended:

```text
Channel Width: 20 MHz
```

The use of 2.4 GHz should be based on actual client and application requirements.

---

### 5 GHz

The 5 GHz band generally provides:

* More available channels
* Better capacity
* Less congestion
* Higher performance

Channel width should be selected based on:

* Client density
* Required capacity
* Available channels
* DFS requirements
* Interference environment

---

### 6 GHz

The 6 GHz band can provide:

* Additional spectrum
* Greater channel availability
* Reduced legacy interference
* Support for newer Wi-Fi technologies

Requirements include:

* Compatible client devices
* Supported AP hardware
* Regulatory compliance
* Appropriate security configuration

The 6 GHz design should consider:

* Channel width
* Client density
* AP placement
* Power levels
* Regulatory restrictions

---

## 11. Data Rate Requirements

The wireless design should define minimum data rate requirements.

Consider:

* Minimum basic rates
* Supported data rates
* Application throughput
* Client capabilities
* Legacy device requirements

Avoid designing the network only around maximum PHY rates.

The effective throughput is influenced by:

```text
PHY Rate
    -
Protocol Overhead
    -
Contention
    -
Retransmissions
    -
Interference
    =
Actual Throughput
```

---

## 12. Coverage Requirements by Application

| Application       |           RSSI Target |            SNR Target | Roaming               |
| ----------------- | --------------------: | --------------------: | --------------------- |
| General Data      |        -67 to -70 dBm |            ≥ 20–25 dB | Normal                |
| Voice             |             ≥ -67 dBm |               ≥ 25 dB | Fast                  |
| Video             |             ≥ -67 dBm |               ≥ 25 dB | Application dependent |
| Barcode Scanner   | Application dependent | Application dependent | Often required        |
| IoT               |      Device dependent |      Device dependent | Usually limited       |
| Location Services |     Based on accuracy |       Based on design | Not always required   |

---

## 13. Physical Environment Considerations

The RF design must account for physical obstructions.

### Building Materials

Consider:

* Concrete
* Reinforced concrete
* Brick
* Drywall
* Glass
* Metal
* Wood
* Insulation
* Water-containing materials

### Special RF Obstacles

Identify:

* Elevators
* Machinery
* Metal shelving
* Storage racks
* Large equipment
* Server racks
* Refrigeration systems
* Industrial equipment

These objects may cause:

* Signal attenuation
* Reflection
* Multipath
* Absorption
* RF shadowing

---

## 14. Vertical Coverage

Multi-floor buildings require vertical coverage analysis.

Consider:

* Floor construction
* Concrete slabs
* Staircases
* Elevator shafts
* AP placement between floors
* RF leakage between floors

The design should not assume that a single AP can reliably cover multiple floors without validation.

---

## 15. Coverage for High-Density Areas

High-density areas should be designed using both coverage and capacity requirements.

Example:

```text
Conference Room
        │
        ├── 100 Users
        ├── 200 Devices
        ├── Voice
        ├── Video
        └── Collaboration Applications
```

The design should consider:

* Number of APs
* Channel reuse
* Channel width
* Transmit power
* Client distribution
* Peak usage

More APs do not automatically mean more capacity.

---

## 16. Coverage for Voice Applications

For voice applications, validate:

* Minimum RSSI
* Minimum SNR
* Roaming performance
* Packet loss
* Latency
* Jitter
* Channel utilization

Example target:

```text
RSSI:       ≥ -67 dBm
SNR:        ≥ 25 dB
Packet Loss: Application dependent
Roaming:    Seamless
```

Actual targets must be confirmed with the voice application and device vendor.

---

## 17. Coverage Validation

Coverage must be validated after implementation.

Validation methods may include:

* Passive survey
* Active survey
* Throughput testing
* Voice testing
* Roaming testing
* Spectrum analysis
* Application testing

The final survey should compare actual results against the design requirements.

---

## 18. Acceptance Criteria

The wireless network should meet the approved coverage targets.

Example:

```text
Coverage:
Required areas achieve the agreed RSSI target.

Signal Quality:
Required areas achieve the agreed SNR target.

Roaming:
Mobile clients can roam according to application requirements.

Capacity:
The design supports the expected number of clients and traffic.

Interference:
Unacceptable RF interference is identified and mitigated.

Application Performance:
Critical applications meet agreed performance requirements.
```

---

## 19. Coverage Exceptions

Any area that does not meet the defined coverage target must be documented.

For each exception, record:

* Location
* Reason
* Current RF performance
* Business impact
* Recommended solution
* Risk
* Customer approval

Example:

```text
Area:
Basement Storage Room

Issue:
Concrete structure causes high attenuation.

Result:
RSSI below the design target.

Recommendation:
Install an additional AP.

Status:
Customer approval required.
```

---

## 20. Recommended Coverage Design Workflow

```text
Define Applications
        │
        ▼
Define RSSI Target
        │
        ▼
Define SNR Target
        │
        ▼
Define Roaming Requirements
        │
        ▼
Analyze Building Materials
        │
        ▼
Perform Survey
        │
        ▼
Design AP Placement
        │
        ▼
Validate Coverage
        │
        ▼
Document Exceptions
        │
        ▼
Customer Acceptance
```

---

## 21. Final Coverage Checklist

* [ ] Coverage areas identified
* [ ] RSSI target defined
* [ ] SNR target defined
* [ ] Noise floor requirements defined
* [ ] Channel utilization requirements defined
* [ ] Roaming requirements defined
* [ ] Voice requirements defined
* [ ] High-density areas identified
* [ ] Outdoor areas identified
* [ ] Physical obstructions documented
* [ ] 2.4 GHz requirements defined
* [ ] 5 GHz requirements defined
* [ ] 6 GHz requirements defined
* [ ] Vertical coverage considered
* [ ] Coverage validation method defined
* [ ] Acceptance criteria approved
* [ ] Coverage exceptions documented

---

## Related Documents


---

## Document Control

| Version | Date       | Author                   | Description     |
| ------- | ---------- | ------------------------ | --------------- |
| 1.0     | YYYY-MM-DD | Network Engineering Team | Initial version |

