# Franka Production 3: Setup Guide

**Document Reference:** R02110 / 1.1 / EN (September 2024)
**Official Manuals:** [www.franka.de/documents](http://www.franka.de/documents)

---

## Table of Contents

1.  [Safety First!](#1-safety-first)
2.  [Prerequisites](#2-prerequisites)
3.  [Unpacking and Preparation](#3-unpacking-and-preparation)
4.  [Physical Installation](#4-physical-installation)
5.  [Wiring and Connections](#5-wiring-and-connections)
6.  [Powering On and Initial Configuration](#6-powering-on-and-initial-configuration)
7.  [Basic Safety Configuration (Watchman)](#7-basic-safety-configuration-watchman)
8.  [End Effector Setup (Optional)](#8-end-effector-setup-optional)
9.  [Advanced Setup & Next Steps](#9-advanced-setup--next-steps)

---

## 1. Safety First!

> **MANDATORY READING:** Before starting **any** setup procedure, thoroughly read and understand **Chapter 4: SAFETY** (Pages 15-34) and **Chapter 9: TRANSPORT AND HANDLING** (Pages 53-54) of the official Product Manual.

**Key Safety Points (Summary - Not Exhaustive):**

*   **Qualified Personnel:** Only qualified or sufficiently trained personnel with adequate technical skills and safety awareness should perform installation and operation (Ref: p.35, p.36).
*   **Intended Use:** Only use the robot for its intended industrial purpose within the specified technical specifications and ambient conditions (Ref: p.16). Misuse voids warranty and is dangerous (Ref: p.16).
*   **Heavy Equipment:** The Arm and Control are heavy. Use correct lifting procedures, personal protective equipment (PPE) like safety shoes, and potentially a second person (Ref: p.53, p.55, p.66, p.68).
*   **Electrical Hazards:** Inspect all components for damage before use. Do not operate damaged equipment. Ensure proper electrical installation and grounding (Ref: p.17, p.53, p.69). Disconnect power before cleaning or maintenance (Ref: p.158).
*   **Mechanical Hazards:** Be aware of potential crushing, pinching, and impact zones during robot motion. Keep clear during operation (Ref: p.17, p.18, p.20).
*   **Emergency Stop:** Ensure the Emergency Stop Device is properly installed, connected to X3.1, and easily accessible (Ref: p.22, p.77-78). Regularly test safety functions (Ref: p.92).
*   **Environment:** Install in a stable, level, vibration-free, indoor environment within specified temperature/humidity ranges. Ensure adequate ventilation (Ref: p.60-63).
*   **Falling Objects:** Secure end effectors and payloads properly. Be aware that power loss or E-Stop can cause objects to fall (Ref: p.18, p.91, p.98, p.99).

---

## 2. Prerequisites

**Before you begin, ensure you have:**

*   **All items from the Scope of Delivery (Chapter 7.1, p.47):**
    *   Arm (FP3)
    *   Control
    *   Connecting Cable (Arm to Control)
    *   Emergency Stop Device
    *   External Enabling Device
    *   Power Cable (country-specific)
    *   Mounting Screws & Washers (M8x20, M5x8, etc.)
    *   Emergency Unlocking Tool
    *   Quick Guide for Installation FP3
*   **Items NOT Included (Chapter 7.2, p.48):**
    *   Interface Device: PC/Laptop/Tablet with Ethernet port and a compatible web browser (Chrome, Firefox, Edge, Safari recommended - Ref: p.94). Minimum resolution 1280x720px, Full HD recommended.
    *   Ethernet Cable (RJ45) for connecting Interface Device to Arm (X5).
    *   (Optional) Ethernet Cable (RJ45) for connecting Control (C2) to shop floor network.
    *   Suitable Baseplate/Mounting Surface (meeting stability requirements - Ref: p.64).
    *   Mounting Hardware (potentially different screws/washers depending on baseplate, check table p.66).
    *   Tools: Hex keys, screwdrivers, torque wrench (30 Nm for Arm mounting - Ref: p.66), spirit level (Ref: p.48, p.64).
    *   Functional Earth Cable (min 1.5 mm² Cu, max 5m - Ref: p.73).
*   **Personnel:** Trained personnel aware of safety procedures (Ref: Section 5, p.35-37).
*   **Documentation:** Access to the full Product Manual (R02110).

---

## 3. Unpacking and Preparation

> **NOTICE:** Handle components carefully. Avoid shocks which can damage sensitive parts. Always keep the original packaging for relocation (Ref: p.53, p.56).

1.  **Inspect Packaging:** Check for external damage upon arrival.
2.  **Environment Check:** Verify the installation site meets the requirements (Ref: Section 10.2, p.60-63):
    *   Indoor, enclosed, no direct sunlight, no vibrations.
    *   Temperature: +5°C to +45°C (Operating).
    *   Humidity: 20% to 80% (non-condensing).
    *   Pollution Degree 2.
    *   Altitude: ≤ 2000m.
    *   Sufficient free workspace (Ref: p.82) and adequate ventilation for Arm and Control (Ref: p.62, p.65).
3.  **Unpack Components:** Carefully follow the unpacking steps illustrated in the manual (Ref: Section 10.1, p.56-59, Figs 10.2-10.11).
    *   Unpack the Arm using the designated lifting points (Ref: p.54, Fig 9.1).
    *   Unpack the Control.
    *   Unpack accessories.
4.  **Prepare Baseplate:** (Ref: Section 10.3.1, p.64, Fig 10.13 & 10.14)
    *   Ensure the mounting surface is stable, level (max tilt 0.1°), non-moving, and can support the robot's static and dynamic forces (see p.64 for forces).
    *   Use the drilling template (Fig 10.14) to prepare mounting holes (4x Ø9mm for M8 screws, 2x Ø6 H7 for optional alignment pins).

---

## 4. Physical Installation

> **WARNING:** Heavy equipment. Use two people and proper lifting techniques/PPE (Ref: p.55, p.66, p.68).
> **NOTICE:** Arm does not stand stable without being screwed to the base (Ref: p.55).

1.  **Mount the Arm:** (Ref: Section 10.4, p.66-67, Fig 10.15)
    *   Lift the Arm using designated points (Fig 9.1).
    *   Carefully position the Arm on the prepared baseplate (use alignment pins if available).
    *   Secure the Arm using four appropriate M8 screws and washers (see table p.66 for screw type based on table material).
    *   Tighten the M8 screws with a torque wrench to **30 Nm**.
    *   Connect the functional earth cable lug to the designated M5 thread on the Arm base (Ref: p.73, Fig 10.20). Secure with M5 tooth washer and M5x8 screw (provided).
2.  **Position the Control:** (Ref: Section 10.5, p.68)
    *   Place the Control horizontally in its intended location (e.g., shelf, 19" rack - 2U required).
    *   Ensure adequate ventilation around the Control (min 40mm clearance for fans - Ref: p.65). Do not block fans.

---

## 5. Wiring and Connections

> **DANGER:** Risk of electric shock from damaged wires or improper installation (Ref: p.17, p.69).
> **WARNING:** Ensure voltages in connected external devices are SELV or suitably isolated (Ref: p.77). Connecting devices with separate power supplies may jeopardize safety if ratings are not met (Ref: p.28, p.77).
> **NOTICE:** Do not swap or unplug the Arm connection (C1/X1) while the Control is powered on (Ref: p.69). Only use connecting cables provided by Franka Robotics (Ref: p.74). Lay cables safely to avoid tripping hazards (Ref: p.69).

**(Refer to Overview Fig 10.1/10.16 and Sections 10.6.1-10.6.4, p.70-77)**

1.  **Arm to Control Cable:**
    *   Connect the **female** end of the connecting cable to port **X1** on the Arm base. Align the triangular marking upwards, insert, and turn the locking ring hand-tight (Ref: p.74, Fig 10.21).
    *   Connect the **male** end of the connecting cable to port **C1** on the Control front panel using the same method (Ref: p.74, Fig 10.22).
2.  **Functional Earth:** Connect the other end of the functional earth cable (from Arm base) to a nearby, well-grounded point (e.g., grounding bar) (Ref: p.73). *This is required for EMC compliance.*
3.  **Emergency Stop Device:** Connect the supplied Emergency Stop Device to port **X3** on the Arm base (Ref: p.22, p.77-78, Fig 4.1, Fig 10.25). Ensure it's placed accessibly but protected from accidental activation. *Custom E-Stop integration must use channel X3.1.*
4.  **External Enabling Device:** Connect the supplied External Enabling Device to port **X4** on the Arm base (Ref: p.75, Fig 10.23). This is needed for Test & Jog mode.
5.  **Interface Device:** Connect your PC/Laptop/Tablet via Ethernet cable to port **X5** on the Arm base (Ref: p.75, p.94).
6.  **(Optional) Shop Floor Network:** Connect the Control (port **C2**) to your company network via Ethernet cable if needed (Ref: p.72, p.153, Fig 14.2).
7.  **Control Power:** Connect the country-specific power cable to port **C3** on the Control rear panel (Ref: p.76, Fig 6.13). Ensure the locking mechanism is used. Connect the other end to the mains supply.

---

## 6. Powering On and Initial Configuration

> **DANGER:** Condensation risk if moving from cold to warm/humid environment. Allow devices to acclimatize before powering on (Ref: p.88).

1.  **Switch On:** Turn on the main power switch on the rear of the Control (Ref: p.88, Fig 11.1).
2.  **Boot Sequence:** (Ref: p.89)
    *   Control fans will start.
    *   Booting takes approx. 1 minute.
    *   Status lights on Arm base and Pilot will flash **slow white**.
    *   Once booted, status lights turn **solid blue** (indicating robot stopped, brakes engaged). Fail-safe locking system is active.
3.  **Connect User Interface:** (Ref: Section 11.3, p.94)
    *   Ensure your interface device (connected to X5) is configured to obtain an IP address via DHCP.
    *   Open a web browser and navigate to `http://robot.franka.de`.
4.  **Initial Configuration ("First Start"):** (Ref: Section 11.4, p.95-98)
    *   The Franka UI "First Start" wizard will appear.
    *   **Language:** Select your preferred language (Fig 11.3). Click NEXT.
    *   **Network:** Review/configure network settings for Robot Network (X5) and Shop Floor Network (C2, optional) (Fig 11.4). The default robot IP is 192.168.0.1. Click NEXT.
    *   **Franka World:** Optionally register the robot with Franka World now (requires internet connection on C2 or via interface device passthrough) or skip (Fig 11.5). Registration is needed for installing Apps/updates later. Click NEXT.
    *   **Administrator User:** Create the initial Administrator user account (username and password) (Fig 11.6). **Store these credentials securely!** Click NEXT.
    *   **End Effector:** Configure the end effector (Fig 11.7). Select "None", "Hand", or "User Defined". If using Franka Hand or another effector, ensure correct parameters (mass, CoM) are entered *later* in Settings for proper operation and safety. **Incorrect configuration can lead to unexpected motion!** (Ref: p.98). Click Confirm.
5.  **Setup Complete:** The Franka UI DESK interface will load. The Arm base lights should remain **solid blue**.

---

## 7. Basic Safety Configuration (Watchman)

> **CRITICAL STEP:** The robot is delivered with pre-validated safety scenarios, but the **"Work" scenario requires configuration and validation by a Safety Operator based on your risk assessment** before automatic operation (Ref: p.25, p.101, p.102). **Operation without proper safety configuration is dangerous.**

1.  **Access Watchman:** Log in as the Administrator created during initial setup. Navigate to Watchman via the main menu. *Note: Only users with the "Safety Operator" role can **edit** safety settings.* The Administrator can create this role in Settings -> Users (Ref: p.37, p.101).
2.  **Understand Scenarios:** Familiarize yourself with the predefined scenarios (Idle, Teach, Test&Jog, Work, Assist, Recovery modes) and their purpose (Ref: p.26-27, p.102).
3.  **Minimum Configuration (Example):** For many basic applications, configuring the safe inputs (X3.2/X3.3) to trigger a stop (e.g., Category 1 Stop or SMSS) when protective devices (light curtains, door switches) are triggered in the "Work" scenario is essential.
4.  **Validation:** **ALL safety configurations, even defaults or minor changes, MUST be validated by the Safety Operator** following the procedure in Chapter 12.6 (p.111-114). This involves testing the functions and generating/signing a Safety Report (Fig 12.21). **The system is not considered safe for operation until validated.**

---

## 8. End Effector Setup (Optional)

1.  **Physical Mounting:** (Ref: Section 10.7, p.78)
    *   Ensure the robot is safely stopped and brakes are engaged or power is off.
    *   Mount the end effector to the Arm's ISO 9409-1-A50 flange (Fig 6.11). Use appropriate screws.
2.  **Electrical Connection:** (Ref: p.72, p.79)
    *   Connect the end effector's cable to the **X6** connector on the Arm's wrist (Fig 10.19). Note the pinout (48V, CAN H/L, GND).
    *   Be aware: X6 power (48V) might be disabled by the `SEEPO` safety function configured in Watchman (Ref: p.29, p.79).
3.  **Software Configuration:** (Ref: p.98, p.105-107)
    *   Log in as Administrator. Go to **Settings -> End Effector**.
    *   Select the correct end effector type ("Hand", "User Defined").
    *   **Crucially, enter accurate Mechanical Data:** Mass, Center of Mass (CoM), Inertia tensor. These values are critical for robot control stability and safety. Refer to the end effector's manual.
    *   **(Advanced):** If using complex end effectors, model its envelope using up to five spheres (Fig 12.8) for accurate safety monitoring (SLP-C, SLS-C).
    *   Configure **SEEPO Behavior** (when the end effector power should be safely cut) and **Power ON Behavior** (Manual/Automatic) in **Watchman -> Safety Setup -> End Effector Configuration** (Ref: p.105-106). *Requires Safety Operator role and re-validation.*

---

## 9. Advanced Setup & Next Steps

Once the basic setup is complete and validated:

*   **User Management:** Create additional users (Operator, Safety Operator) in **Settings -> Users** (Ref: p.37, p.134).
*   **Franka World:** Fully register the robot (if not done earlier) and link it to your Franka World account to manage Apps and Updates (**Settings -> Franka World**) (Ref: Chapter 14, p.152-154).
*   **Network Configuration:** Finalize shop floor network settings (static IP, DNS) if needed (**Settings -> Network**) (Ref: p.156).
*   **Advanced Safety (Watchman):** Implement detailed safety rules and scenarios (Cartesian limits, speed limits) based on your full risk assessment (**Watchman -> Edit Scenarios**) (Ref: p.108-113). *Requires Safety Operator role.*
*   **Backup:** Perform a full manual backup of the configuration (Safety Report PDF, Network screenshots, Modbus JSON, End effector JSON, Task files) (Ref: Section 14.5, p.155-157).
*   **Programming:** Start creating Tasks using Apps in **DESK** (Ref: Section 13.6, p.135).
*   **Regular Testing:** Remember to perform regular tests of safety functions (Ref: Section 11.2.2, p.92).

---
