| [Home](https://github.com/fortinet-fortisoar/solution-pack-brute-force-attack-response/tree/release/1.0.1/README.md) |
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution packs that appears, search for and select **Brute Force Attack Response**.
3. Click the **Brute Force Attack Response** solution pack card.
4. Click **Install** on the bottom to begin installation.

## Prerequisites

|Solution Pack Name|Purpose|
| :- | :- |
|SOAR Framework 1.0.0|Required for Incident Response modules|
|SOC Simulator 1.0.1|Required for Scenario Module and SOC Simulator connector|

# Configuration

For optimal performance of **Brute Force Attack Response** solution pack, you can install and configure:

- Threat intelligence connectors to enrich context of a given indicator
    - To configure and use the VirusTotal connector as a source of threat intelligence, refer to [Configuring Virus Total](https://docs.fortinet.com/document/fortisoar/2.1.0/virustotal/166/virustotal-v2-1-0#Configuration_parameters)
- A data ingestion process to periodically search and read events, alerts, and other notables from a data source and convert them into actionable items, such as alerts, in FortiSOAR
    - To configure and use the Splunk connector for data ingestion, refer to [Configuring Splunk Connector](https://docs.fortinet.com/document/fortisoar/1.6.2/splunk/130/splunk-v1-6-2#Configure_Data_Ingestion)
- A directory service to retrieve information about users, groups, and computers, in an organization
    - To configure and use the Active Directory connector as a directory service, refer to [Configuring Active Directory Connector](https://docs.fortinet.com/document/fortisoar/2.2.0/active-directory/154/active-directory-v2-2-0#Configuration_parameters)