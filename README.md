# Wazuh SIEM & File Integrity Monitoring Lab

## Overview
I used Wazuh to monitor file changes in a personal lab and investigate the resulting alerts. I created, modified, and deleted a test file, then reviewed the events in the Wazuh dashboard.

The goal was to understand how a file change becomes a security alert and what an analyst needs to check before drawing a conclusion.

## Lab Environment
- macOS host
- VMware Fusion running Ubuntu Server
- Wazuh security monitoring platform
- Linux and macOS command-line tools

## Work Performed
- Edited the Wazuh monitoring configuration to specify a directory to watch.
- Adjusted monitoring settings and restarted the relevant service.
- Created, modified, and deleted a test file.
- Located the resulting file integrity monitoring alerts in the Wazuh dashboard.
- Reviewed file paths, timestamps, agent details, rule descriptions, and available file hashes.

## Alert Investigation
For each event, I checked:
- Which endpoint reported the change
- Which file was affected
- Whether the file was created, modified, or deleted
- When Wazuh recorded the event
- What additional details were available to explain the change

A file change alert shows that a monitored change occurred. It does not, by itself, establish who made the change or whether the activity was malicious.

## Results and Lessons Learned
The original exercise produced alerts for the test file's creation, modification, and deletion.

I learned how monitoring configuration affects visibility and how to examine an alert beyond its title. I also learned to separate what the event proves from what still requires investigation.

## Supporting Evidence
Screenshots and configuration details will be added after review to confirm the monitored endpoint, file path, and settings used in the original exercise
