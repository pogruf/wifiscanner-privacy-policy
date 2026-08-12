# Privacy Policy for "Wi-Fi Scanner"

**Effective Date:** August 13, 2026

This Privacy Policy describes how the "Wi-Fi Scanner" mobile application (hereinafter referred to as the "Application") handles user information. The Application is designed as a local tool for wireless network auditing and network security analysis.

We value your privacy and **DO NOT collect, transmit, or store** your personal or network data on any external servers.

---

## 1. Permissions Requested and Their Purpose

To perform its functions, the Application requires the following Android system permissions:

*   **Access to Location (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`):** Required by the Android operating system to legally scan the radio spectrum (retrieving SSIDs and BSSIDs of surrounding Wi-Fi networks). Without this permission, Android blocks access to the Wi-Fi scanning APIs. The Application **does not** track or record your actual physical coordinates.
*   **Notifications (`POST_NOTIFICATIONS`):** Used on Android 13+ to deliver local system notifications (e.g., warnings about detected network threats or scan completion events).
*   **Network and Wi-Fi Access:** Required to send ICMP requests (Ping), check TCP/UDP ports within your local subnet, and read the network neighbor cache (Netlink/ARP).

---

## 2. Data Collection, Storage, and Transfer

*   **Local Storage Only:** All scan results (connection history, lists of discovered devices, their IP/MAC addresses, and open ports) are saved exclusively within a local SQLite database (`DbHelper`) on your device.
*   **No Backend Server:** The Application does not use any remote servers. We do not collect telemetric analytics, and we do not share your network data with any third parties.
*   **Data Deletion:** You can completely clear your scan history at any time by clearing the Application's storage in the Android system settings or by uninstalling the Application.

---

## 3. Data Security

Because all operations are performed locally on your device, the security of your data depends on the security of the device itself. We use standard, secure system APIs (Java 17 / Android SDK) to interact with the Linux kernel network stack.

---

## 4. Changes to This Privacy Policy

We may periodically update this Privacy Policy as new features are added. All changes will be published on this GitHub page with an updated effective date.

---

## 5. Contact Information

If you have any questions regarding the Application or this Policy, you can open an Issue in this GitHub repository.
