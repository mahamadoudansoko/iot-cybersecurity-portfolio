# Project 1: Smart Building Security System with Intrusion Detection

## 🏢 Overview
A comprehensive IoT-based security system for a 3-floor commercial building featuring automated intrusion detection, network segmentation, and real-time monitoring.

## 🎯 Objectives
- Implement network segmentation for IoT devices (5 VLANs)
- Configure wireless security protocols (WPA2-PSK)
- Design automated security response systems
- Deploy surveillance and access control mechanisms

## 🛠️ Technologies Used
- **Platform:** Cisco Packet Tracer 8.2+
- **Devices:** 
  - Motion Sensors (9)
  - Door Sensors (6)
  - Smart Locks (3)
  - IP Cameras (6)
  - Wireless Access Points (3)
- **Network:** VLAN segmentation, inter-VLAN routing, ACLs, port security

## 📋 Key Features
- ✅ 5-VLAN network architecture (Management, IoT, Cameras, Users, Servers)
- ✅ WPA2-PSK wireless security with AES encryption
- ✅ Automated intrusion response (motion detection → door locking)
- ✅ Centralized security monitoring and logging
- ✅ Port security with MAC address limiting
- ✅ Access Control Lists (ACLs) for traffic isolation

## 📂 Project Structure
\\\
01-smart-building-ids/
├── packet-tracer/       # .pkt files
├── docs/               # Technical documentation
├── configs/            # Router/Switch configurations
├── screenshots/        # Topology & testing screenshots
├── reports/            # Final reports & presentations
└── tests/              # Test scenarios & results
\\\

## 🚀 Quick Start
1. Open \SmartBuilding-Security-System.pkt\ in Cisco Packet Tracer
2. Review network topology and VLAN assignments
3. Test intrusion detection scenarios (see \	ests/\ folder)
4. Access security dashboard at 192.168.50.10

## 📊 Network Architecture
- **Management VLAN 10:** 192.168.10.0/24
- **IoT Sensors VLAN 20:** 192.168.20.0/24
- **Security Cameras VLAN 30:** 192.168.30.0/24
- **User Devices VLAN 40:** 192.168.40.0/24
- **Servers VLAN 50:** 192.168.50.0/24

## 🔒 Security Controls Implemented
| Control | Status | Description |
|---------|--------|-------------|
| Network Segmentation | ✅ | 5 VLANs with strict isolation |
| Wireless Security | ✅ | WPA2-PSK with unique SSIDs per floor |
| Access Control Lists | ✅ | Server & IoT traffic filtering |
| Port Security | ✅ | MAC address restrictions |
| Automated Response | ✅ | Event-driven door locking |
| Centralized Logging | ✅ | Syslog server for audit trail |

## 📈 Testing Results
All test scenarios passed successfully:
- ✅ Ground floor intrusion detection
- ✅ First floor after-hours access
- ✅ Server room breach prevention
- ✅ Network isolation verification

## 🎓 Skills Demonstrated
- Network design & VLAN segmentation
- IoT security architecture
- Wireless security configuration
- Access control implementation
- Security automation
- Incident response workflows

## 🔗 CYBERUS Programme Alignment
This project directly aligns with CYBERUS curriculum themes:
- **IoT Security:** Device isolation, wireless hardening
- **Network Security:** ACLs, VLANs, port security
- **Critical Infrastructure:** Building automation systems
- **Incident Response:** Automated threat mitigation

## 📝 Documentation
- [Technical Architecture](docs/architecture.md)
- [Configuration Guide](docs/configuration-guide.md)
- [Test Scenarios](tests/test-plan.md)
- [Final Report](reports/final-report.pdf)

## 👤 Author
**Mahamadou DANSOKO**  
Cybersecurity Solutions Integration Engineer  
DATAPROTECT, Casablanca  
[GitHub](https://github.com/mahamadoudansoko) | [LinkedIn](#)

## 📅 Project Timeline
- **Start Date:** [Your Start Date]
- **Completion Date:** [Your Completion Date]
- **Duration:** 10 days

## 📜 License
This project is part of an academic portfolio for the CYBERUS Erasmus Mundus Programme application.

---
*Project developed as part of IoT Cybersecurity specialization portfolio*
