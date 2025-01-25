<h1>Nessus</h1>

<h2>Description</h2>

<p>In this project, I designed a hands-on guide to performing vulnerability assessments using Nessus, a popular and powerful vulnerability scanner. The project is tailored for beginners to help them gain practical experience in identifying, analyzing, and prioritizing security vulnerabilities in a target system or network.</p>

<h2>Pre-requisites</h2>

- Basic understanding of network and system administration
- Familiarity with Linux command line
- A computer with a Linux-based operating system (preferably Ubuntu)
- Nessus Home or Professional license (Nessus Home is free for personal use)

<h2>Lab Set-up and Tools</h2>

- Ubuntu 20.04 or later
- Nessus installed (instructions provided in the first task)
- A target machine for scanning (can be a local VM or a networked device)

<h2>Task 1: Installing Nessus</h2>

1. Download the Nessus installation package from the Tenable website:
   ```bash
   wget https://www.tenable.com/downloads/api/v1/public/pages/nessus/downloads/XXXX/download?i_agree_to_tenable_license_agreement=true
   ```
2. Install Nessus using the downloaded package:
   ```bash
   sudo dpkg -i <name-of-downloaded-file>.deb
   ```
3. Start the Nessus service:
   ```bash
   sudo systemctl start nessusd
   ```
4. Enable the Nessus service to start automatically on boot:
   ```bash
   sudo systemctl enable nessusd
   ```
5. Open the Nessus web interface by navigating to ``https://<your-ip>:8834`` in your browser.

**Expected Outcome:**

- Nessus will be successfully installed and running, and you’ll be able to access its web interface to proceed with the initial setup.

## Task 2: Configuring Nessus for Scanning

1. Log in to the Nessus web interface.
2. Complete the initial setup by creating an admin account and activating Nessus with the provided activation code.
3. Navigate to the Settings section to configure optional proxy settings or enable updates.

**Expected Outcome:**

- Nessus will be fully configured and ready to create custom scan policies and scanning tasks.

## Task 3: Creating a Scan Policy

1. In the Nessus web interface, go to the Policies section.
2. Click New Policy to create a custom scan policy.
3. Choose a policy template that fits your scanning needs (e.g., Basic Network Scan).
4. Customize the policy by adding details such as the scan name, description, and target preferences.
5. Save your newly created policy.

**Expected Outcome:**

- The scan policy is created and saved, ready to be applied for targeted scanning.

## Task 4: Running a Vulnerability Scan

1. Navigate to the Scans section in the Nessus web interface.
2. Click New Scan and select the policy created in the previous step.
3. Enter the scan details, such as a name for the scan and the target IP address.
4. Save the scan configuration and click Launch to start the scan.

**Expected Outcome:**

- The scan begins, and you can monitor its progress and review preliminary results in real-time.

## Task 5: Analyzing Scan Results

1. Once the scan is complete, open the completed scan in the Scans section.
2. Review the scan results, paying attention to identified vulnerabilities, their severity levels, and recommended remediation steps.
3. Export the scan report in your preferred format (e.g., PDF, HTML) for documentation and further analysis.

**Expected Outcome:**

- A detailed scan report is generated, highlighting vulnerabilities, their severity, and actionable remediation recommendations.
