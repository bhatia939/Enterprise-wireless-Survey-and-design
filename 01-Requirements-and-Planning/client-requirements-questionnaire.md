# Client Requirements Questionnaire

This questionnaire is used to collect the business, technical, application, user, security, and environmental requirements needed to design an enterprise wireless network.

---

## 1. General Information

| Question                     | Response |
| ---------------------------- | -------- |
| Organization / Customer Name |          |
| Project Name                 |          |
| Site / Location              |          |
| Contact Person               |          |
| IT Contact                   |          |
| Business Owner               |          |
| Planned Deployment Date      |          |

---

## 2. Business Requirements

### 2.1 What is the primary objective of this wireless project?

* [ ] New wireless deployment
* [ ] Existing WLAN upgrade
* [ ] Coverage improvement
* [ ] Capacity improvement
* [ ] Performance improvement
* [ ] Technology refresh
* [ ] Migration to a new wireless platform
* [ ] Other: __________

### 2.2 How business-critical is the wireless network?

* [ ] Low
* [ ] Medium
* [ ] High
* [ ] Mission-critical

### 2.3 What is the required network availability?

```text
Target Availability: ______________________
Planned Maintenance Window: _______________
```

---

## 3. Site and Building Information

| Question                  | Response |
| ------------------------- | -------- |
| Number of Buildings       |          |
| Number of Floors          |          |
| Total Area                |          |
| Ceiling Height            |          |
| Construction Type         |          |
| Wall Materials            |          |
| Floor Materials           |          |
| Metal Structures          | Yes / No |
| Industrial Equipment      | Yes / No |
| Outdoor Coverage Required | Yes / No |

### Building Materials

* [ ] Drywall
* [ ] Concrete
* [ ] Brick
* [ ] Glass
* [ ] Metal
* [ ] Reinforced Concrete
* [ ] Other: __________

---

## 4. User and Device Requirements

### 4.1 How many users will use the wireless network?

```text
Total Users: __________________
Peak Concurrent Users: ________
```

### 4.2 How many wireless devices are expected?

```text
Total Wireless Devices: ________
Peak Concurrent Devices: ______
```

### 4.3 What types of devices will be used?

* [ ] Laptops
* [ ] Smartphones
* [ ] Tablets
* [ ] Voice Handsets
* [ ] Barcode Scanners
* [ ] IoT Devices
* [ ] Printers
* [ ] Medical Devices
* [ ] Industrial Devices
* [ ] BYOD Devices
* [ ] Other: __________

---

## 5. Application Requirements

### Which applications will use the wireless network?

* [ ] Web / Internet
* [ ] Voice over Wi-Fi
* [ ] Video Conferencing
* [ ] Microsoft Teams
* [ ] Cloud Applications
* [ ] ERP
* [ ] Warehouse Management
* [ ] Point of Sale
* [ ] Healthcare Applications
* [ ] Industrial Applications
* [ ] IoT
* [ ] Other: __________

### Application Requirements

| Application | Number of Users | Bandwidth | Latency Sensitive | Roaming Required |
| ----------- | --------------: | --------- | ----------------- | ---------------- |
|             |                 |           | Yes / No          | Yes / No         |
|             |                 |           | Yes / No          | Yes / No         |
|             |                 |           | Yes / No          | Yes / No         |

---

## 6. Wireless Coverage Requirements

### Which areas require coverage?

* [ ] Offices
* [ ] Meeting Rooms
* [ ] Corridors
* [ ] Reception
* [ ] Cafeteria
* [ ] Warehouse
* [ ] Production Area
* [ ] Outdoor Area
* [ ] Parking Area
* [ ] Loading Dock
* [ ] Stairwell
* [ ] Elevator Area

### Coverage Requirement

```text
Required Minimum RSSI: __________________
Required Minimum SNR: ___________________
Required Minimum Data Rate: _____________
```

---

## 7. Capacity Requirements

### Expected Client Density

| Area | Users | Wireless Clients | Peak Concurrent Clients |
| ---- | ----: | ---------------: | ----------------------: |
|      |       |                  |                         |
|      |       |                  |                         |
|      |       |                  |                         |

### High-Density Locations

* [ ] Auditorium
* [ ] Conference Room
* [ ] Classroom
* [ ] Training Room
* [ ] Cafeteria
* [ ] Event Area
* [ ] Warehouse
* [ ] Other: __________

---

## 8. Roaming Requirements

Is seamless roaming required?

* [ ] No
* [ ] Yes
* [ ] Voice roaming
* [ ] Video roaming
* [ ] Warehouse mobility
* [ ] Healthcare mobility
* [ ] Industrial mobility

### Required Technologies

* [ ] 802.11k
* [ ] 802.11v
* [ ] 802.11r
* [ ] Fast BSS Transition

---

## 9. Wireless Security Requirements

### Authentication

* [ ] WPA2-Personal
* [ ] WPA2-Enterprise
* [ ] WPA3-Personal
* [ ] WPA3-Enterprise
* [ ] 802.1X
* [ ] Certificate-Based Authentication
* [ ] PSK
* [ ] MPSK
* [ ] MAC Authentication Bypass

### Authentication Platform

* [ ] Aruba ClearPass
* [ ] Cisco ISE
* [ ] Microsoft NPS
* [ ] Other: __________

### Access Control

* [ ] Dynamic VLAN Assignment
* [ ] Dynamic Role Assignment
* [ ] Device Profiling
* [ ] Guest Access
* [ ] BYOD
* [ ] IoT Segmentation
* [ ] Network Access Control

---

## 10. SSID Requirements

| SSID      | Purpose | Users / Devices | Authentication | Security |
| --------- | ------- | --------------- | -------------- | -------- |
| Corporate |         |                 |                |          |
| Guest     |         |                 |                |          |
| IoT       |         |                 |                |          |
| Voice     |         |                 |                |          |

### SSID Design Considerations

* [ ] Minimize unnecessary SSIDs
* [ ] Separate corporate and guest access
* [ ] Segment IoT devices
* [ ] Apply role-based access
* [ ] Define appropriate QoS
* [ ] Define authentication method

---

## 11. Network Integration

### Existing Network Infrastructure

| Component         | Vendor / Model | Version | Details |
| ----------------- | -------------- | ------- | ------- |
| Wireless Platform |                |         |         |
| Switches          |                |         |         |
| Routers           |                |         |         |
| Firewall          |                |         |         |
| Authentication    |                |         |         |
| Monitoring        |                |         |         |

### Integration Requirements

* [ ] VLAN Integration
* [ ] DHCP
* [ ] DNS
* [ ] RADIUS
* [ ] Active Directory
* [ ] PKI
* [ ] SIEM
* [ ] Network Monitoring
* [ ] API Integration

---

## 12. Power and Cabling

| Requirement              | Response                    |
| ------------------------ | --------------------------- |
| PoE Available            | Yes / No                    |
| PoE Standard             | 802.3af / 802.3at / 802.3bt |
| Cable Category           |                             |
| Cable Length Limitations |                             |
| Existing Network Closets |                             |
| New Cabling Required     | Yes / No                    |

---

## 13. Future Requirements

What growth is expected?

* [ ] More users
* [ ] More wireless devices
* [ ] IoT expansion
* [ ] Wi-Fi 6E adoption
* [ ] Wi-Fi 7 adoption
* [ ] New buildings
* [ ] Higher bandwidth requirements
* [ ] Location services
* [ ] Other: __________

### Expected Growth

```text
Expected User Growth: ____________________
Expected Device Growth: __________________
Expected Timeline: _______________________
```

---

## 14. Survey Requirements

### Survey Type Required

* [ ] Predictive Survey
* [ ] Passive Survey
* [ ] Active Survey
* [ ] AP-on-a-Stick Survey
* [ ] Spectrum Analysis
* [ ] Post-Deployment Validation

### Survey Tool

```text
Survey Tool: _____________________________
Survey Engineer: _________________________
Planned Survey Date: _____________________
```

---

## 15. Client Requirements Summary

### Critical Requirements

1. ---
2. ---
3. ---

### Business-Critical Applications

1. ---
2. ---
3. ---

### Key Design Constraints

1. ---
2. ---
3. ---

---

## 16. Customer Confirmation

The information provided in this questionnaire represents the current wireless requirements and will be used as input for the wireless design and survey process.

| Role                    | Name | Signature | Date |
| ----------------------- | ---- | --------- | ---- |
| Customer Representative |      |           |      |
| IT Representative       |      |           |      |
| Network Architect       |      |           |      |

---

> **Important:** Wireless design recommendations should be based on confirmed business, application, client, coverage, capacity, security, and environmental requirements.

