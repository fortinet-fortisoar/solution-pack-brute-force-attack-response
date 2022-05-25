| [Home](https://github.com/fortinet-fortisoar/solution-pack-brute-force-attack-response/blob/develop/README.md) |
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution pack that appears, search for and select **Brute Force Attack Response**.
3. Click the **Brute Force Attack Response** solution pack card.
4. Click **Install** on the bottom to begin installation.

## Prerequisites

|Solution Pack Name|Purpose|
| :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector|

# Configuration

# Configuration

For optimal performance of **Brute Force Attack Response** solution pack, you can install and configure:

* Threat intelligence connectors to enrich context of a given indicator
    * To configure and use the VirusTotal connector as a source of threat intelligence, refer to [Configuring Virus Total](https://docs.fortinet.com/document/fortisoar/2.1.0/virustotal/166/virustotal-v2-1-0#Configuration_parameters)
* A data ingestion process to periodically search and read events, alerts, and other notables from a data source and convert them into actionable items, such as alerts, in FortiSOAR
    * To configure and use the Splunk connector for data ingestion, refer to [Configuring Splunk Connector](https://docs.fortinet.com/document/fortisoar/1.6.2/splunk/130/splunk-v1-6-2#Configure_Data_Ingestion)
