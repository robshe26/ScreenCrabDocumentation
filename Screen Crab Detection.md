
# Screen Crab Detection Analysis

This document outlines the primary indicators for detecting a Screen Crab device on a target PC when no Wi-Fi connection is active.

### Overview: Non-Wireless Detection
In environments where **Wi-Fi is disabled**, detection relies on identifying discrepancies in how the operating system recognizes and renders the display output.

---

## Technical Comparison: Connected vs. Disconnected

The following table summarizes the key visual and technical indicators identified when a Screen Crab is inline between the host and the monitor.

| Feature | Screen Crab Connected | Direct Connection (Standard) |
| :--- | :--- | :--- |
| **Monitor Name** | Identified as `Wired Display` | Identified as `HDMI TV` |
| **Refresh Rate** | Restricted (See Hz settings) | Native/Standard Refresh Rate |
| **Display Scaling** | Noticeable scaling variance | Standard system scaling |

---

## Detailed Detection Indicators

### 1. Display Identification
The most immediate indicator is found within the system display settings. The Screen Crab identifies itself as a generic display interface rather than the actual hardware connected.

* **Connected Status:** The OS lists the monitor as a **Wired Display**.
    <img width="1007" height="297" alt="ScreenCrab - Display" src="https://github.com/user-attachments/assets/9e6e5411-5916-4838-b100-b003f66cea40" />

* **Disconnected Status:** The OS correctly identifies the monitor as an **HDMI TV**.
    <img width="1007" height="297" alt="ScreenCrab - Display" src="https://github.com/user-attachments/assets/dd0b2717-ea47-4bcd-8f38-898e2fe90bfd" />

### 2. UI Scaling Discrepancies
A visible change in the desktop scale occurs when the Screen Crab is active. This is often caused by the device's internal capture resolution hardware intercepting the signal.

* **With Screen Crab:**
    <img width="1919" height="1079" alt="ScreenCrab-Conntedhome" src="https://github.com/user-attachments/assets/30f9dbdc-fa59-4663-aaae-0919a996edca" />

* **Direct Connection:**
    <img width="1919" height="1079" alt="ScreenCrab - Home" src="https://github.com/user-attachments/assets/d36fcb56-afcb-4790-b090-57c847ffb12e" />

### 3. Refresh Rate (Hz) Limitations
The Screen Crab hardware supports a specific range of refresh rates. Comparing the available frequency options (Hz) can reveal the presence of the device.

* **Connected:** Frequency options are restricted or altered.

    <img width="202" height="456" alt="ScreenCrab-ConnectedHTZ" src="https://github.com/user-attachments/assets/b8ee9661-cb1f-4045-b78f-9699b1d858f2" />

* **Disconnected:** Full range of native refresh rates is available.

    <img width="129" height="232" alt="Screencrab - HTZ" src="https://github.com/user-attachments/assets/f403f4a6-b25b-4b2d-8378-acc5aee46580" />






























