# Test Plan - Smart Building Security System
# ==========================================

## Test Environment
- **Platform:** Cisco Packet Tracer 8.2.2
- **Test Date:** [Insert Date]
- **Tester:** Mahamadou DANSOKO

## Test Scenarios

### Test 1: Ground Floor Intrusion Detection
**Objective:** Verify automated response to unauthorized entry

**Preconditions:**
- All sensors operational
- Smart lock in unlocked state
- Security monitoring active

**Steps:**
1. Activate Motion-Ground-Entrance sensor
2. Open Door-Ground-Main sensor
3. Observe automated response

**Expected Results:**
- Lock-Ground-Main activates within 2 seconds
- Alert sent to Security-Monitor-PC
- Event logged on Security-Control-Server

**Status:** [ ] PASS  [ ] FAIL

---

### Test 2: Network Isolation Verification
**Objective:** Verify VLAN segmentation and ACL enforcement

**Steps:**
1. From IoT-Hub-Ground (192.168.20.10), ping Security-Monitor-PC (192.168.40.10)
2. From Camera-Ground-Entrance (192.168.30.10), ping IoT-Hub-Ground
3. From Security-Monitor-PC, ping Security-Control-Server (192.168.50.10)

**Expected Results:**
- IoT → User VLAN: BLOCKED by ACL
- Camera → IoT: BLOCKED by ACL
- User → Server: ALLOWED

**Status:** [ ] PASS  [ ] FAIL

---

### Test 3: Wireless Security
**Objective:** Verify WPA2-PSK authentication

**Steps:**
1. Attempt connection with incorrect passphrase
2. Attempt connection with correct passphrase
3. Verify encrypted communication

**Expected Results:**
- Incorrect passphrase: Connection rejected
- Correct passphrase: Connection successful
- Traffic encrypted with AES

**Status:** [ ] PASS  [ ] FAIL

---

### Test 4: Port Security
**Objective:** Verify MAC address restrictions

**Steps:**
1. Connect authorized device to camera port
2. Disconnect and connect unauthorized device
3. Observe port behavior

**Expected Results:**
- Authorized device: Port remains active
- Unauthorized device: Port shuts down
- Security violation logged

**Status:** [ ] PASS  [ ] FAIL

---

### Test 5: Server Room Critical Zone
**Objective:** Verify enhanced security for critical infrastructure

**Steps:**
1. Trigger Motion-Second-ServerRoom
2. Trigger Door-Second-Server
3. Verify immediate lockdown

**Expected Results:**
- Instant lock activation
- High-priority alert generated
- Camera recording triggered

**Status:** [ ] PASS  [ ] FAIL

---

## Test Results Summary

| Test ID | Scenario | Status | Response Time | Notes |
|---------|----------|--------|---------------|-------|
| T1 | Ground Floor Intrusion | | | |
| T2 | Network Isolation | | | |
| T3 | Wireless Security | | | |
| T4 | Port Security | | | |
| T5 | Server Room Protection | | | |

## Issues & Observations
[Document any issues encountered during testing]

## Recommendations
[List any improvements or fixes needed]

---
**Approved By:** _______________  
**Date:** _______________
