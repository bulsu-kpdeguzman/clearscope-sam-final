# ClearScope BIM - Enterprise 3D Network Campus Walkthrough

An interactive, realistic 3D architectural digital twin and network walkthrough visualization built with Three.js.

## Overview
This interactive application visualizes the complete campus network infrastructure for ClearScope Technologies across 4 main facilities:
- **Employees' Building:** 5 stories, 100 workstations (VLAN 10, `10.10.10.0/24`)
- **Studio Server Room & Server Farm:** Core Catalyst 3650 switch, Cisco Firepower NGFW, PLDT/Globe edge routers, and dedicated Employee & Admin Server PCs (VLAN 30, `192.168.30.0/24`)
- **Administration Building:** 2 floors, 30 workstations (VLAN 20, `192.168.20.0/24`)
- **Second Branch Office:** 2 floors, 35 workstations (VLAN 50 & 60, `192.168.50.0/24` & `192.168.60.0/24`)

## Features
- **Realistic Architectural Campus Model:** Pitched gabled slate roofs, warm stucco walls, vertical timber cladding accents, paved walkways, landscaped lawn, trees, and parked cars (Zero grid lines).
- **1-Click Style Switcher:** Toggle instantly between **Campus (Realistic Daylight)** and **Studio (Pristine White Gallery)**.
- **Interactive Network Packet Simulations:**
  1. *Employee PC to Server:* Smooth drone chase camera glides inside Room 101 tracking the packet out through the doorway and across the campus conduit into the Server Room.
  2. *Block Guest Access:* Visualizes Cisco Firepower ACL 110 intercepting and dropping unauthorized guest traffic at the firewall.
  3. *Main to Branch Leased Line:* High-speed WAN sync over a 500 Mbps CIR private point-to-point link.
  4. *Branch Direct Internet:* Direct DIA internet routing through the Cisco 2911 ISR branch router.
  5. *Failover (HSRP):* Simulates primary PLDT carrier outage and instant sub-3-second failover to Globe Business.
- **Dual Navigation Modes:**
  - **Orbit Mode:** Smooth 3D CAD orbit, pan, and zoom.
  - **Walk Mode:** First-person architectural walkthrough with physical keyboard (`WASD`) on desktop, and a touch virtual joystick on mobile devices.
- **Mobile Responsive:** Swipeable facility navigation bar, adaptive bottom dock, and slide-up bottom sheets.
- **100% Offline Compatible:** Zero external npm or CDN build steps required.

## Deployment on GitHub Pages
1. Push this repository to GitHub.
2. In your repository, go to **Settings** > **Pages**.
3. Under **Build and deployment** > **Branch**, select `main` (or `master`) and `/ (root)`.
4. Click **Save**. GitHub Pages will automatically host the 3D walkthrough via `index.html`.
