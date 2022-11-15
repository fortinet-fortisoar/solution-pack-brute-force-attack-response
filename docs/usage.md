| [Home](../README.md) | 
|----------------------| 

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/usage.md) to understand how to simulate and reset scenarios.

To understand the process FortiSOAR follows to respond to brute force attack attempts, we have included a scenario &mdash; **Brute Force Attempt** with this solution pack. Refer to the section *Brute Force Attempt* to understand how this solution pack's automation addresses your needs.

## Brute Force Attempt

This scenario generates a demo alert of type **Brute Force Attempt** from the **Syslog** connector.

Navigate to the demo alert and note the following:

- The demo alert created is an example of a default data ingestion using the **Data Ingestion** feature
- The alert is of type *Brute Force Attempts*
- The reported alert contains the following among other related sources data:
    - Source IP address
    - Destination IP address
    - Destination port
    - Targeted asset details

## Brute Force Attempt (FortiSIEM)

This scenario generates a demo alert of type **Brute Force Attempt** from the **FortiSIEM** connector.

Navigate to the demo alert and note the following:

- The demo alert created is an example of a default data ingestion using the **Data Ingestion** feature
- The alert is of type *Brute Force Attempts*
- The reported alert contains the following among other related sources data:
    - Source IP address
    - Destination IP address
    - Process name
    - Computer name (hostname) details

Users can launch the following playbooks:
- Investigate Brute Force
- Investigate Brute Force (FortiSIEM)

These playbooks perform the following automated tasks:

- If the source IP address found is internal, mark the IP address as benign
- If the source IP found is external:
    - Gets the reputation of the source IP address using VirusTotal connector
    - Retrieves additional details about source IP from Splunk or Active Directory
    - Block the IP address as part of the Brute Force Attack remediation process
