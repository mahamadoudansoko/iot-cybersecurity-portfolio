# Project 1 — Smart Building Security System with Intrusion Detection

## 🏢 Overview

A comprehensive IoT-based security system for a 3-floor commercial building, simulated in **Cisco Packet Tracer 8.2+**, featuring automated intrusion detection, VLAN network segmentation, and real-time centralized monitoring.

---

## 🎯 Objectives

- Implement network segmentation for IoT devices using 5 VLANs
- Configure wireless security protocols (WPA2-PSK + AES)
- Design automated security response systems (motion → lock)
- Deploy surveillance and access control mechanisms across 3 floors

---

## 🛠️ Technologies Used

- **Platform:** Cisco Packet Tracer 8.2+
- **Network Devices:** Cisco 4331 Router, Cisco 3650-24PS Switch (PoE)
- **IoT Devices:** Motion Sensors (9), Door Sensors (6), Smart Locks (3), IP Cameras (6), Wireless Access Points (3)
- **Security:** VLAN segmentation, inter-VLAN routing, ACLs, port security, Syslog

---

## 📋 Key Features

- ✅ 5-VLAN network architecture (Management, IoT-Sensors, Cameras, Users, Servers)
- ✅ WPA2-PSK wireless security with AES encryption per floor
- ✅ Automated intrusion response — motion detection triggers smart lock
- ✅ Centralized Syslog monitoring on Security-Control-Server
- ✅ Port security with sticky MAC address limiting
- ✅ ACLs for server protection and IoT traffic isolation

---

## 📂 Project Structure

```
01-smart-building-ids/
├── packet-tracer/       # .pkt simulation file
├── docs/                # Network plan, architecture notes, build log
├── configs/             # Router and switch CLI configurations
├── screenshots/         # Topology and testing evidence per phase
├── reports/             # Security matrix and final writeup
├── tests/               # Test plan and results
└── scripts/             # Python automation scripts
```

---

## 🚀 Quick Start

1. Open `SmartBuilding-Security-System.pkt` in Cisco Packet Tracer 8.2+
2. Review the network topology and VLAN assignments
3. Run intrusion detection test scenarios (see `tests/test-plan.md`)
4. Access the security dashboard at `192.168.50.10`

---

## 📊 Network Architecture

| VLAN | Name             | Subnet            | Gateway         |
|------|------------------|-------------------|-----------------|
| 10   | Management       | 192.168.10.0/24   | 192.168.10.254  |
| 20   | IoT-Sensors      | 192.168.20.0/24   | 192.168.20.254  |
| 30   | Security-Cameras | 192.168.30.0/24   | 192.168.30.254  |
| 40   | User-Devices     | 192.168.40.0/24   | 192.168.40.254  |
| 50   | Servers          | 192.168.50.0/24   | 192.168.50.254  |

---

## 🔒 Security Controls Implemented

| Control | Status | Description |
|---------|--------|-------------|
| Network Segmentation | ✅ | 5 VLANs with strict isolation |
| Wireless Security | ✅ | WPA2-PSK with unique SSIDs per floor |
| Access Control Lists | ✅ | PROTECT-SERVERS + ISOLATE-IOT on router |
| Port Security | ✅ | Sticky MAC address restrictions on camera ports |
| Automated Response | ✅ | Event-driven door locking on intrusion detection |
| Centralized Logging | ✅ | Syslog server for full audit trail |
| Physical Access Control | ✅ | Smart locks on all 3 floors |
| Surveillance | ✅ | 6 IP cameras across all security zones |

---

## 🏗️ Security Zones

| Zone          | Floor  | Security Level | Key Devices                      |
|---------------|--------|----------------|----------------------------------|
| Public Zone   | Ground | Low            | Lobby sensors, entrance camera   |
| Restricted    | First  | Medium         | Office sensors, conference room  |
| Critical Zone | Second | High           | Server room, executive offices   |

---

## 📈 Testing Results

| Test | Scenario | Status |
|------|----------|--------|
| T1 | Ground floor intrusion detection | ✅ Pass |
| T2 | Network isolation (ACL verification) | ✅ Pass |
| T3 | Wireless WPA2-PSK authentication | ✅ Pass |
| T4 | Port security on camera ports | ✅ Pass |
| T5 | Server room critical zone response | ✅ Pass |

> Full test details available in [`tests/test-plan.md`](tests/test-plan.md)

---

## 🎓 Skills Demonstrated

- Network design and VLAN segmentation
- IoT security architecture
- Wireless security configuration
- Access control list (ACL) implementation
- Security automation and event-driven response
- Incident response workflows and centralized logging

---

## 📝 Documentation

- [Network Plan](docs/network-plan.md)
- [Build Log](docs/build-log.md)
- [Switch Configuration](configs/switch-config.txt)
- [Router Configuration](configs/router-config.txt)
- [Test Plan](tests/test-plan.md)
- [Security Matrix](reports/security-matrix.md)

---

## 👤 Author

**Mahamadou DANSOKO**  
Cybersecurity Solutions Integration Engineer  
DATAPROTECT, Casablanca  
[GitHub](https://github.com/mahamadoudansoko) | [LinkedIn](#)

---

## 📅 Project Timeline

- **Start Date:** [Your Start Date]
- **Completion Date:** [Your Completion Date]
- **Duration:** ~10 days

---

## 📜 License

This project is part of an academic cybersecurity portfolio.  
See [LICENSE](../../LICENSE) for details.

---

*Part of the [IoT Cybersecurity Portfolio](../../README.md)*