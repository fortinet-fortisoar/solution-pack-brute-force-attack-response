| [Home](../README.md) | 
|----------------------| 

# Contents

## Connectors

| Connector Name             | Description                                                                                                                                                       |
|:---------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| VirusTotal                 | Scans and analyzes suspicious files, URLs, IP addresses and retrieves reports from VirusTotal about them                                                          |
| Splunk                     | Helps users invoke search, fetch events to related search, invoke alert actions, update notables, sync splunk users to FortiSOAR etc.                             |
| Microsoft Active Directory | Helps directly query AD to retrieve information about users, groups, and computers, in an organization, by using the Lightweight Directory Access Protocol (LDAP) |

> **WARNING:** After deployment, this Solution Pack installs or upgrades the stated list of connectors.

## Global Variable

| Global Variable | Description                               |
|:----------------|:------------------------------------------|
| `Demo_mode`     | Enables playbook to execute a mock output |

## Record Sets

| Scenario                      | Description                                                                                                                               |
|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------|
| Brute Force Attack            | This scenario demonstrates a typical Multiple Login Failure, detected using the **Syslog** connector, on an asset exposed to internet.    |
| Brute Force Attack(FortiSIEM) | This scenario demonstrates a typical Multiple Login Failure, detected using the **FortiSIEM** connector, on an asset exposed to internet. |

## Playbook Collections

| 02 - Use Case - Brute Force Attack |
|:-----------------------------------|

| Playbook Name                                   | Description                                                                                                                                                                |
|:------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Investigate Brute Force Attempt                 | Investigates login failures and also identifies other impacted assets that have been victims of the brute force attempts from a particular source of attack                |
| Investigate Brute Force Attempt (FortiSIEM)     | Investigates login failures from FortiSIEM and also identifies other impacted assets that have been victims of the brute force attempts from a particular source of attack |
| Scenario - FortiSIEM (Brute Force Attack) Alert | Generates a demo alert for Brute Force Attack                                                                                                                              |

>**WARNING:** It is recommended to clone these playbooks before making any customizations to avoid loss of information while upgrading the solution pack.

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
|-----------------------------------------|-------------------------------------------|---------------------|