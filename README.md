<h1>Nessus</h1>

<h2>Description</h2>

<p>This project involves learning and utilizing the Nexus Essentials Vulnerability Scanner, a free and widely-used tool for identifying security vulnerabilities in networks. The scanner automates the detection of issues like outdated software and default passwords across up to 16 devices, providing detailed reports ranked by severity using the CVSS framework. Participants will install, configure, and run scans to practice identifying and remediating vulnerabilities, ensuring a secure network environment.</p>

<h2>Requirements</h2>

- Operating System:
  - Windows 10 or later (64-bit)
  - macOS 10.15 or later
  - Various Linux distributions (e.g., Ubuntu, CentOS, Debian)
- Hardware:
  - Minimum 2 GHz CPU
  - At least 4 GB RAM (8 GB recommended for larger networks)
  - 20 GB available disk space
- Browser:
  - Chrome, Firefox, Edge, or Safari to access the Nessus interface via ``https://localhost:8834``
- Internet Connection:
  - Required for downloading the installer, plugins, and updates.
- Account Registration:
  - A valid email address to register and receive the activation code for Nessus Essentials.

## Understand the Purpose of Vulnerability Scanners

- Vulnerability scanners automate the process of identifying vulnerabilities (e.g., missing updates, default passwords) on a network.
- They rank vulnerabilities by severity to prioritize fixes.

## Task 1: Download the Nexus Essentials Scanner

1. Open a browser and search for "Nexus Essentials Vulnerability Scanner."
2. Visit the Tenable website, fill in the required fields (first name, last name, email), and click "Get Started."
3. Follow the link sent to your email to download the software.
4. Choose the appropriate version for your system (e.g., Windows x86 64-bit).

## Task 2: Install the Scanner

1. Launch the installer after downloading.
2. Select the default installation options (no custom changes needed).
3. Allow the software to download and install required plugins (this process may take 30–40 minutes).

## Task 3: Access the Scanner

1. The scanner is accessed via a web browser.
2. Open a browser and navigate to ``https://localhost:8834``.
3. Save the URL for easy access later.

## Task 4: Set Up the Scanner

1. Register the software using the activation code sent to your email.
2. Create a username and password to log in.
3. Use a strong password (e.g., "P@ssw0rd").

## Task 5: Find Your Network Details

1. Open the Command Prompt:
   - Press ``Win + R``, type ``cmd``, and press Enter.
   - Type ipconfig and note the following:
     - IP Address: (e.g., ``10.0.2.15``)
     - Subnet Mask: (e.g., ``255.255.255.0``, indicating a /24 network).
     - Determine the network ID: e.g., ``10.0.2.0/24``.

## Task 6: Create a New Scan

1. Log in to the scanner via your browser (``https://localhost:8834``).
2. Select the option to create a new scan and choose a "Basic Network Scan."
3. Name your scan (e.g., "My Home Network").
4. Enter the network ID (e.g., ``10.0.2.0/24``).
5. Save the scan configuration.

## Task 7: Run the Scan

1. Launch the scan and wait for it to complete.
2. Scanning time will vary based on network size and resources.

## Task 8: Review the Results

1. Once the scan is complete, review the findings:
   - Informational: General details; no immediate action required.
   - Low/Medium/High/Critical: Assess these vulnerabilities based on severity and prioritize fixes.
2. Click on each vulnerability to view details (e.g., outdated software, default passwords).

## Task 9: Remediate Vulnerabilities

1. Address vulnerabilities based on severity:
   - Critical/High: Fix immediately (e.g., update software, reset default passwords).
   - Medium/Low: Address as time permits.
2. For outdated machines: Run Windows Update or apply necessary patches.

## Task 10: Ongoing Use

1. Keep the software installed to regularly scan your network (up to 16 devices for free).
2. Regularly check for software updates to ensure the scanner is up-to-date.

## Key Points to Remember

- The scanner uses the CVSS (Common Vulnerability Scoring System) to rank vulnerabilities.
- Save the scanner’s access URL (``https://localhost:8834``) with the correct protocol (HTTPS).
- The software is free for up to 16 devices and can be used for both personal and small office networks.
