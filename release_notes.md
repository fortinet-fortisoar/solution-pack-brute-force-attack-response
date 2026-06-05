# What's New

## Enhancements

- *Incident* has been renamed to **Case**.

## Fixes

- The playbook *Investigate Brute Force Attempt* is now available for use in the list of *Alerts*' and *Cases*' **Execute** button.

- In the event of a **Brute Force Attempt** Case record, if the VirusTotal's `last_analysis_stats.malicious` score for the source IP address is greater than zero, the case record severity will be automatically escalated to Critical. Additionally, the same source IP address will be submitted for blocking through the manual input process.
