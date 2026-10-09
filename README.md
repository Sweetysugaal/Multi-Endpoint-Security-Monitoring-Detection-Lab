# Multi-Endpoint Security Monitoring & Detection Lab

## Overview

This project is a cybersecurity proof of concept demonstrating how security telemetry from multiple Windows endpoints can be collected centrally, analyzed, and investigated using Elastic Security.

The lab focuses on endpoint monitoring, security detection, alert investigation, and dashboard visibility.

## Objectives

- Collect Windows security telemetry centrally.
- Monitor PowerShell activity and process execution.
- Configure Sysmon and Windows event logging.
- Test security detection rules using controlled, benign activity.
- Investigate alerts and review supporting event evidence.
- Visualize security activity through an Elastic dashboard.

## Tools and Technologies

- Elastic Security
- Elastic Agent
- Windows 10 virtual machines
- Sysmon
- Windows Event Logging
- PowerShell Script Block Logging
- Oracle VirtualBox

## Architecture

Windows endpoints generate security events. Elastic Agent collects the configured telemetry and forwards it to the central Elastic environment, where the data can be searched, visualized, and analyzed by detection rules.

**Workflow:**

Windows Endpoints → Event Collection → Elastic Security → Detection Rules → Alerts → Investigation

## Detection and Investigation

The lab includes testing and reviewing detection capabilities related to:

- PowerShell script block activity
- Encoded PowerShell command arguments
- Windows process execution
- Custom detection rules using controlled test activity

Alerts are investigated using available evidence such as the affected host, timestamp, process, command line, and underlying event.

An alert is an indicator that activity requires investigation; it is not, by itself, proof of compromise.

## Dashboard

The Elastic dashboard provides an overview of event activity, monitored hosts, alert severity, and recent security alerts.

## Key Learning Outcomes

- Centralized security telemetry collection
- SIEM search and dashboard development
- Detection-rule testing
- Security alert investigation
- Endpoint logging and monitoring
- Documentation of a security proof of concept

## Limitations

This is a lab-based proof of concept, not a production SOC deployment. Detection results depend on the configured data sources, rules, and test activity. Additional validation, security controls, and operational procedures would be required for production use.

## Future Improvements

- Expand endpoint and network telemetry sources.
- Improve and document detection test cases.
- Add investigation procedures and response playbooks.
- Improve separation and organization of endpoint data.
- Document further testing results and lessons learned.

## Author

**Zeinab Ali Mohamed**

Cybersecurity | Blue Team | Security Monitoring | SIEM
