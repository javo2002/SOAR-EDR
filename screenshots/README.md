# SOAR-EDR Project Screenshots

This directory contains screenshots documenting the setup, configuration, and execution of the **SOAR-EDR (Security Orchestration, Automation, and Response for Endpoint Detection and Response)** project. Below is a description of each screenshot in order:

---

## Screenshot 1.png
- **Content**: Overview of the SOAR-EDR playbook workflow.
- **Details**: 
  - The playbook includes steps for handling alerts, such as sending messages with details (time, computer name, source IP, process, command line, file path, sensor ID, and detection link).
  - User prompts for isolating computers and updating communication platforms (Slack, Email).

<p align="center">
  <img src="./images/Screenshot 1.png" alt="screenshot 1" width="600">
</p>

---

## Screenshot 2.png
- **Content**: Cloud OS provisioning in the Vultr environment.
- **Details**: 
  - Configuration of a Windows 2022 server for simulating an infected machine.
  - Firewall settings to restrict access via RDP (port 3389).

<p align="center">
  <img src="./images/Screenshot 2 2.png" alt="screenshot 2" width="600">
</p>

---

## Screenshot 3.png
- **Content**: Firewall configuration for the Vultr cloud environment.
- **Details**: 
  - Inbound IPv4 rules to secure the VM.
  - Rules for allowing specific protocols and ports (e.g., RDP on port 3389).

<p align="center">
  <img src="./images/Screenshot 3 2.png" alt="screenshot 3" width="600">
</p>

---

## Screenshot 4.png
- **Content**: Remote connection initiation to the Windows 2022 server.
- **Details**: 
  - Connecting to the VM via IP address `155.138.221.95`.

<p align="center">
  <img src="./images/Screenshot 4 2.png" alt="screenshot 4" width="600">
</p>

---

## Screenshot 4a.png
- **Content**: Successful installation of the LimaCharlie agent.
- **Details**: 
  - The LimaCharlie agent is installed on the Windows 2022 server.
  - Confirmation message: "Agent installed successfully!"

<p align="center">
  <img src="./images/Screenshot 4a 2.png" alt="screenshot 4a" width="600">
</p>

---

## Screenshot 4b.png
- **Content**: Execution of the Lazagne tool on the Windows 2022 server.
- **Details**: 
  - Lazagne is used to simulate credential dumping.
  - Output includes decrypted system masterkeys and password hashes.

<p align="center">
  <img src="./images/Screenshot 4b 2.png" alt="screenshot 4b" width="600">
</p>

---

## Screenshot 6.png
- **Content**: LimaCharlie sensor configuration.
- **Details**: 
  - Sensor details for the Windows 2022 server (`javi-soar-edr`).
  - Real-time event collection and artifact monitoring.

<p align="center">
  <img src="./images/Screenshot 6 2.png" alt="screenshot 6" width="600">
</p>

---

## Screenshot 7.png
- **Content**: Detection events in LimaCharlie.
- **Details**: 
  - Detections related to processes, file integrity, and network activity.
  - Example: Detection of `LaZagne.exe` and related processes.

<p align="center">
  <img src="./images/Screenshot 7 2.png" alt="screenshot 7" width="600">
</p>

---

## Screenshot 8.png
- **Content**: Detection rule configuration in LimaCharlie.
- **Details**: 
  - Rules for identifying suspicious processes and activities.
  - Example: Rule to detect the execution of `LaZagne.exe`.

<p align="center">
  <img src="./images/Screenshot 8 2.png" alt="screenshot 8" width="600">
</p>

---

## Screenshot 9.png
- **Content**: Detection report metadata.
- **Details**: 
  - Report for the detection of `LaZagne.exe`.
  - Metadata includes author, description, and tags (e.g., `attack.credential_access`).

<p align="center">
  <img src="./images/Screenshot 9 2.png" alt="screenshot 9" width="600">
</p>

---

## Screenshot 10.png
- **Content**: Output configuration in LimaCharlie.
- **Details**: 
  - Integration of LimaCharlie with Tines for automated workflows.
  - Stream detections and events to external tools (e.g., Slack, S3).

<p align="center">
  <img src="./images/Screenshot 10 2.png" alt="screenshot 10" width="600">
</p>

---

## Screenshot 11.png
- **Content**: Story configuration in Tines.
- **Details**: 
  - Story setup for the SOAR-EDR project.
  - Includes credentials for Slack and LimaCharlie integrations.

<p align="center">
  <img src="./images/Screenshot 11 2.png" alt="screenshot 11" width="600">
</p>

---

## Screenshot 12.png
- **Content**: Detection alert email.
- **Details**: 
  - Email notification for the detection of `LaZagne.exe`.
  - Includes details such as computer name, source IP, file path, and detection link.

<p align="center">
  <img src="./images/Screenshot 12 2.png" alt="screenshot 12" width="600">
</p>

---

## Screenshot 13.png
- **Content**: Sensor details in LimaCharlie.
- **Details**: 
  - Information about the `javi-soar-edr` sensor.
  - Includes hostname, platform, network access, and sensor ID.

<p align="center">
  <img src="./images/Screenshot 13 2.png" alt="screenshot 13" width="600">
</p>

---

## Screenshot 14.png
- **Content**: Tines workflow execution.
- **Details**: 
  - Detection alert and isolation workflow in Tines.
  - Includes user prompts and confirmation of computer isolation.

<p align="center">
  <img src="./images/Screenshot 14 2.png" alt="screenshot 14" width="600">
</p>

---

## Screenshot 14a.png
- **Content**: Tines workflow diagram.
- **Details**: 
  - Workflow steps for retrieving detections, sending emails, and user prompts.
  - Includes HTTP requests and actions for isolation status.

<p align="center">
  <img src="./images/Screenshot 14a 2.png" alt="screenshot 14a" width="600">
</p>

---

## Screenshot 15.png
- **Content**: Updated sensor details after isolation.
- **Details**: 
  - Sensor status shows the computer is isolated from the network.
  - Option to rejoin the network after investigation.

<p align="center">
  <img src="./images/Screenshot 15 2.png" alt="screenshot 15" width="600">
</p>

---

This README provides a high-level overview of the screenshots and their relevance to the SOAR-EDR project. For more details, refer to the individual screenshots and the associated documentation.
