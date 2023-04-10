# Release Information

* **Version**:  1.2.0
* **Certified**: Yes
* **Publisher**: Fortinet
* **Compatible Version**: FortiSOAR v7.2.0 and above
* [Release Notes](./release_notes.md)

# Overview

The **Brute Force Attack Response Solution Pack** investigates login failures and also identifies other impacted assets that have been victims of the brute force attempts from a particular source of attack.

You can configure ingestion using connectors such as **FortiSIEM** and **Syslog**. The ingestion process creates an alert of type **Brute Force Attempts** and then triggers the response workflow.

The use-case deals with a typical *Multiple Login Failure* on an asset exposed to internet.

* Fields of interest (Source and Destination IP address) are extracted as indicators and enriched
* The playbook &mdash; Investigate Brute Force Attempt &mdash; illustrates a step-by-step response plan

# Next Steps

| [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) |
|--------------------------------------------|----------------------------------------------|------------------------|------------------------------|
