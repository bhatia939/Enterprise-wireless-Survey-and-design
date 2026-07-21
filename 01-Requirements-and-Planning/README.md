# 01 - Requirements and Planning

Wireless design should begin with a clear understanding of business, technical, application, user, and environmental requirements.

A well-defined requirements phase helps ensure that the wireless network is designed for the actual business needs rather than only for basic coverage.

---

## 🎯 Objectives

The objectives of this phase are to:

* Understand business requirements
* Identify wireless applications
* Determine coverage requirements
* Determine capacity requirements
* Identify client device types
* Define performance targets
* Understand security requirements
* Identify environmental constraints
* Define survey requirements

---

## 📋 Requirements Collection Process

```text
Business Requirements
        │
        ▼
Application Requirements
        │
        ▼
Client & Device Requirements
        │
        ▼
Coverage & Capacity Requirements
        │
        ▼
Security Requirements
        │
        ▼
Environmental Assessment
        │
        ▼
Wireless Design Requirements
```

---

## 🏢 Business Requirements

Understand how the wireless network supports the business.

Important questions:

* What areas require wireless coverage?
* Is wireless the primary network access method?
* How critical is wireless connectivity?
* What is the expected network availability?
* Are there business-critical wireless applications?
* Are there future expansion requirements?

---

## 📱 Application Requirements

Identify applications that will use the wireless network.

Examples:

* Voice over Wi-Fi
* Video conferencing
* Real-time collaboration
* Point-of-Sale systems
* Barcode scanners
* Healthcare applications
* Industrial IoT
* Warehouse applications
* Guest Internet access
* Location services

Each application may have different requirements for:

* Bandwidth
* Latency
* Packet loss
* Roaming
* Availability
* Security

---

## 👥 User and Client Requirements

Collect information about:

* Number of users
* Number of wireless clients
* Client types
* Client capabilities
* Expected concurrent users
* Device density
* BYOD requirements
* IoT device requirements

Example:

```text
Location: Open Office

Users: 150
Expected Wireless Clients: 350
Concurrent Clients: 250
Voice Devices: 30
IoT Devices: 50
Guest Clients: 100
```

---

## 📶 Coverage Requirements

Define the required coverage area.

Examples:

* Office areas
* Meeting rooms
* Corridors
* Warehouses
* Production areas
* Outdoor areas
* Parking areas
* Loading docks

Define the required coverage targets based on the application.

Example:

| Application       |           RSSI Target |            SNR Target |
| ----------------- | --------------------: | --------------------: |
| General Data      |               -67 dBm |                 25 dB |
| Voice             |               -67 dBm |                 25 dB |
| High-Density Data |               -65 dBm |                 25 dB |
| IoT               | Application dependent | Application dependent |

These values should always be validated against the specific application and client requirements.

---

## 📊 Capacity Requirements

Coverage alone does not guarantee a good wireless network.

Capacity planning should consider:

* Number of users
* Number of clients
* Concurrent devices
* Application bandwidth
* AP client capacity
* Channel width
* Available spectrum
* Channel utilization

A high-density area may require additional APs even when the signal strength is excellent.

---

## 🔐 Security Requirements

Define security requirements such as:

* WPA2-Enterprise
* WPA3-Enterprise
* 802.1X authentication
* Certificate-based authentication
* Guest access
* BYOD
* IoT segmentation
* Network access control
* Dynamic role assignment
* VLAN segmentation

Example platforms:

* Aruba ClearPass
* Cisco ISE
* RADIUS
* PKI
* Identity-based access control

---

## 🏗️ Environmental Requirements

The physical environment has a significant impact on RF performance.

Document:

* Building construction
* Wall materials
* Floor materials
* Ceiling height
* Metal structures
* Glass walls
* Concrete walls
* Machinery
* Elevators
* Storage racks
* Production equipment

Example:

```text
Concrete Wall
      │
      ▼
High RF Attenuation
      │
      ▼
Reduced Coverage
      │
      ▼
Additional AP Required
```

---

## 🗺️ Required Site Information

Before starting the survey, collect:

* Floor plans
* Building drawings
* Ceiling plans
* Floor dimensions
* Wall construction details
* AP mounting restrictions
* Network room locations
* Cable pathways
* Existing AP locations
* Existing wireless survey results

---

## ✅ Planning Checklist

* [ ] Business requirements collected
* [ ] Application requirements identified
* [ ] User density identified
* [ ] Client device types identified
* [ ] Coverage requirements defined
* [ ] Capacity requirements defined
* [ ] Security requirements defined
* [ ] Building construction documented
* [ ] Floor plans collected
* [ ] Survey areas identified
* [ ] Wireless design targets approved

---

## 📂 Related Files

* `wireless-requirements.md`
* `client-requirements-questionnaire.md`
* `application-requirements.md`
* `survey-planning-checklist.md`

---

> **Design Principle:** A successful wireless network begins with understanding the business and application requirements before selecting AP models or placing access points.

