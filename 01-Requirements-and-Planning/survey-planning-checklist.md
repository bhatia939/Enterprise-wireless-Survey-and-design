# Wireless Survey Planning Checklist

This checklist provides a structured process for planning an enterprise wireless site survey before visiting the site or starting data collection.

---

# 1. Project Information

* [ ] Project name defined
* [ ] Customer / organization identified
* [ ] Site location confirmed
* [ ] Primary technical contact identified
* [ ] Business owner identified
* [ ] Survey engineer assigned
* [ ] Survey date confirmed
* [ ] Survey scope documented

```text
Project Name: ___________________________
Customer: _______________________________
Site: ___________________________________
Survey Engineer: _________________________
Survey Date: ____________________________
```

---

# 2. Business Requirements

* [ ] Business objectives documented
* [ ] Wireless-critical business services identified
* [ ] Required network availability documented
* [ ] Future growth requirements documented
* [ ] Business-critical areas identified
* [ ] Business priorities confirmed

---

# 3. Site Information

* [ ] Building information collected
* [ ] Number of buildings confirmed
* [ ] Number of floors confirmed
* [ ] Floor areas documented
* [ ] Ceiling heights documented
* [ ] Building construction documented
* [ ] Wall materials identified
* [ ] Metal structures identified
* [ ] Industrial equipment identified
* [ ] Outdoor coverage areas identified

---

# 4. Floor Plans

* [ ] Current floor plans received
* [ ] Floor plans verified against actual site
* [ ] Floor plans are to scale
* [ ] Floor dimensions confirmed
* [ ] Walls and rooms identified
* [ ] Restricted areas identified
* [ ] AP mounting locations identified
* [ ] Network closets identified
* [ ] Cable pathways identified

### Required Floor Plan Formats

* [ ] PDF
* [ ] DWG
* [ ] DXF
* [ ] Image
* [ ] Other: __________

---

# 5. User and Client Requirements

* [ ] Total users identified
* [ ] Concurrent users identified
* [ ] Total wireless devices identified
* [ ] Client device types documented
* [ ] Device density documented
* [ ] BYOD requirements identified
* [ ] IoT devices identified
* [ ] Voice devices identified
* [ ] High-density areas identified

---

# 6. Application Requirements

* [ ] Business applications identified
* [ ] Voice requirements identified
* [ ] Video requirements identified
* [ ] Warehouse applications identified
* [ ] IoT applications identified
* [ ] Latency-sensitive applications identified
* [ ] Bandwidth requirements documented
* [ ] Roaming requirements documented
* [ ] QoS requirements documented

---

# 7. Wireless Design Targets

Define the required performance targets.

| Metric                      | Target |
| --------------------------- | ------ |
| Minimum RSSI                |        |
| Minimum SNR                 |        |
| Maximum Noise Floor         |        |
| Maximum Channel Utilization |        |
| Minimum Data Rate           |        |
| Maximum Packet Loss         |        |
| Maximum Latency             |        |

Example:

```text
RSSI:              -67 dBm or better
SNR:                25 dB or better
Noise Floor:       -85 dBm or lower
Channel Utilization: < 50%
Packet Loss:        < 1%
```

---

# 8. Existing Wireless Environment

* [ ] Existing APs identified
* [ ] Existing WLAN platform identified
* [ ] Existing controller / cloud platform identified
* [ ] Existing SSIDs documented
* [ ] Existing RF profiles documented
* [ ] Existing wireless issues documented
* [ ] Existing survey results collected
* [ ] Existing coverage maps reviewed

---

# 9. RF Environment

* [ ] 2.4 GHz environment reviewed
* [ ] 5 GHz environment reviewed
* [ ] 6 GHz requirements reviewed
* [ ] External interference considered
* [ ] Non-Wi-Fi interference considered
* [ ] Noise sources identified
* [ ] DFS requirements considered
* [ ] Regulatory domain confirmed

---

# 10. Survey Type Selection

Select the required survey type.

* [ ] Predictive Survey
* [ ] Passive Survey
* [ ] Active Survey
* [ ] AP-on-a-Stick Survey
* [ ] Spectrum Analysis
* [ ] Post-Deployment Validation

---

# 11. AP-on-a-Stick Preparation

If performing an APoS survey:

* [ ] AP model selected
* [ ] AP firmware confirmed
* [ ] Survey configuration prepared
* [ ] Survey SSID configured
* [ ] Survey authentication configured
* [ ] PoE injector prepared
* [ ] PoE battery prepared
* [ ] AP mounting equipment prepared
* [ ] Tripod / pole prepared
* [ ] Mounting height confirmed

---

# 12. Survey Equipment

### Wireless Equipment

* [ ] Survey AP
* [ ] Spare AP
* [ ] PoE injector
* [ ] PoE battery
* [ ] Ethernet cable
* [ ] Console cable

### Survey Equipment

* [ ] Survey laptop
* [ ] Survey software
* [ ] Wi-Fi adapters
* [ ] Spectrum analyzer
* [ ] Measuring tape
* [ ] Laser distance meter
* [ ] Camera
* [ ] Floor plans

### Safety Equipment

* [ ] Safety shoes
* [ ] High-visibility vest
* [ ] Helmet if required
* [ ] Site-specific PPE

---

# 13. Survey Software

```text
Survey Software: _________________________
Version: __________________________________
Operating System: ________________________
Survey Adapter: __________________________
```

Examples:

* Ekahau
* NetSpot
* AirMagnet
* WiFi Explorer
* Wireshark
* Kismet

---

# 14. Site Access

* [ ] Site access approved
* [ ] Security requirements confirmed
* [ ] Visitor registration completed
* [ ] Access badge arranged
* [ ] Working hours confirmed
* [ ] Escort requirements confirmed
* [ ] Restricted areas identified
* [ ] Safety induction completed

---

# 15. Survey Execution Plan

Define the survey workflow.

```text
Site Arrival
     │
     ▼
Site Validation
     │
     ▼
Floor Plan Verification
     │
     ▼
RF Environment Assessment
     │
     ▼
AP-on-a-Stick Placement
     │
     ▼
Survey Data Collection
     │
     ▼
Application Testing
     │
     ▼
Data Review
     │
     ▼
Survey Report
```

---

# 16. Survey Data to Collect

* [ ] RSSI
* [ ] SNR
* [ ] Noise Floor
* [ ] Channel Utilization
* [ ] Co-Channel Interference
* [ ] Adjacent-Channel Interference
* [ ] PHY Data Rate
* [ ] Throughput
* [ ] Packet Loss
* [ ] Latency
* [ ] Roaming Performance

---

# 17. Post-Survey Activities

* [ ] Survey data reviewed
* [ ] Coverage gaps identified
* [ ] Capacity issues identified
* [ ] Interference identified
* [ ] AP locations finalized
* [ ] AP quantity confirmed
* [ ] Channel plan reviewed
* [ ] Transmit power reviewed
* [ ] Design recommendations documented
* [ ] Final survey report created

---

# 18. Final Readiness Check

Before starting the survey:

* [ ] Requirements approved
* [ ] Floor plans available
* [ ] Survey scope confirmed
* [ ] Survey tools ready
* [ ] Survey equipment ready
* [ ] APoS configuration tested
* [ ] Site access confirmed
* [ ] Safety requirements confirmed
* [ ] Survey targets defined
* [ ] Survey schedule confirmed

---

> **Survey Principle:** Proper planning reduces survey errors, improves data quality, and ensures that the final wireless design reflects actual business, application, RF, and environmental requirements.

