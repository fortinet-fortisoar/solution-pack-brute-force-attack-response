# Usage Brute Force Attack Solution Pack
# Use Case Workflow

This solution pack contains two types of execution workflows
* Scenario-based Workflow
* Investigate Brute Force Attack
* Investigate Brute Force Attack (FortiSIEM)

##  Scenario-based Workflow

The scenario demonstrates and generates a demo alert for the Alert Type **Brute Force Attempts**.

The Scenario-based workflow follows the following pattern:
1. Go to the **Simulations** menu in Navigation and choose Device **Brute Force Attempt** and **Brute Force Attempt (FortiSIEM)**.
2. Click on the **Run Scenario** button to create demo records for the scenario.
4. The created Alerts records IRI will be displayed in the Scenario record.

## Investigate Brute Force Attempts

After the scenario workflow generates the demo alert, the use case workflow investigates it through a playbook.

![Investigation playbook](media/BFAR-investigation-playbook.png)

The investigation playbooks follow the following pattern:

1. Manual trigger of the playbook starts the investigation on 'Brute Force Attempt' alert for source 'syslog' and looks for any malicious IOC (Indicator of Compromise) related to the alert.

    ![Manual Execution Trigger](media/BFAR-manual-execution-trigger.png)

2. If it finds a malicious IOC, it updates the alert severity to critical and checks if the target system is Windows or Linux.
    * Windows:
        * Gets details from Active Directory
    * Linux:
        * Query Splunk for related events for source IP address
        * Create and link affected assets
3. If the IOC found is non-malicious IOC, it marks the IP as safe.

## Investigate Brute Force Attempts(FortiSIEM)

After the scenario workflow generates the demo alert, the use case workflow investigates it through a playbook.

![FortiSIEM Investigation playbook](media/BFAR-FortiSIEM-investigation-playbook.png)

The investigation playbooks follow the following pattern:

1. Manual trigger of the playbook starts the investigation on **Brute Force Attempt**. The alert is **Sudden Increase in Failed Logins To A Host**, and the source is **FortiSIEM**.   
2. It then looks for any malicious IOC related to the alert.
3. If it finds a malicious IOC, it updates the alert's severity to critical and checks for a manual intervention to block the IP address.
    * When it receives instructions to block
        * It gets IOC details
        * It blocks the IOC
    * When it receives instructions to allow
        * It creates a note to allow the IP address
4. If the IP address found is non-malicious, it creates a note marking the IP as safe.