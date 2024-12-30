# Security-splunk
 
Introduction

This repository showcases my work on the “Asset and Inventory Management” course-end project. The primary goal was to resolve a permissions issue within Splunk, applying skills in file system navigation, risk management, digital forensics, and system administration.

Project Overview
Scenario:

At StackFull Software, a Splunk configuration file (config.conf) was inadvertently modified by a junior analyst, preventing access to logs.
My task was to locate the file, fix the permissions, verify integrity using md5sum, update the file, and create a backup.
Key Steps:

Locate the correct config.conf within /opt/splunk.
Check & record file permissions.
Compute MD5 hashes before and after editing.
Edit & save the file to add user credentials:
plaintext
Copy code
[admin]
AliceAdmin1
[YourName]Admin2
Back up config.conf to /home/fstack.
Report the findings and recommendations to leadership.
Learning Objectives
Asset & Inventory Management

Navigate the file system and manage file permissions in Linux.
Create, move, delete files/directories, and use sorting/formatting tools.
Risk Management

Identify potential risks & vulnerabilities related to misconfigurations.
Recognize how confidentiality, integrity, and availability (CIA) can be compromised.
Digital Forensics

Use hashing (md5sum) to verify file integrity.
Understand how logs feed into a SIEM for incident resolution.
System Administration

Automate maintenance tasks and manage user accounts and groups.
Adjust configurations to meet security needs.
Interpersonal Skills

Communicate effectively with colleagues, using active listening and clear instructions.
Work collaboratively to troubleshoot and solve technical issues.
Problem Solving

Practice a “security mindset” to identify assets, adversaries, threats, and weaknesses.
Apply inductive/deductive reasoning to implement and evaluate solutions.
Writing

Produce clear, organized, and logical reports, tailored to the appropriate audience.
Document modifications for forensic and audit purposes.
The Permissions Problem: Summary
Problem:
A misconfigured config.conf file in Splunk prevented proper log viewing and posed a security risk due to incorrect permissions.

Solution:
Located the file, updated permissions to secure confidentiality, and added new admin user lines. Verified the file’s integrity using md5sum both before and after edits. Made a backup to prevent data loss and allow rollback if needed.

Confidentiality Improvement:
Ensured only authorized SOC analysts could modify the configuration by adjusting ownership and file permissions. Recommended ongoing permission audits.

Integrity Monitoring:
Emphasized running md5sum regularly or automating integrity checks on critical Splunk files. This helps quickly identify unauthorized or accidental changes.

Repository Structure
plaintext
Copy code
.
├── README.md               # Project overview (this file)
├── report.pdf (or .md)     # Detailed findings and recommendations
├── scripts/                # Any scripts or commands used
└── docs/
    └── Project_Details.md  # Extended scenario details (if desired)
How to Use
Clone the repository:
bash
Copy code
git clone https://github.com/<YourGitHubUsername>/<YourRepoName>.git
Explore the code and documentation to see how each step was performed.
Practice the instructions and replicate the tasks in a Linux environment (VM or sandbox).# Security-splunk
 
