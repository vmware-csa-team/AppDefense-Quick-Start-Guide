---
layout: single
title: "Discovery Mode"
permalink: /workshop-manual/
date: 2019-05-20
tags: workshop
classes: wide
author_profile: false
---
## What is Discovery Mode? 

In Discovery Mode AppDefense creates a list of allowed behaviors to build a blueprint or a birth certificate of the natural state of the application.(Please note we recommend staying in discovery mode for at least 14 days) 

## What is the Purpose of Discovery Mode? 
This mode helps AppDefense to understand how the application must function so that AppDefense can identify malicious or unintended behaviors.

## What is learned in Discovery Mode? 
- Processes: Standard executeable of an application. (svchost.exe is a standard executeable of a Microsoft service)
- Behaviors: Process executions (CLIs) and network activities (inbound and outbound connections) exhibited within a service.

## Viewing Behaviors 

On the "Behaviors" tab, click the behavior that you want to view.

You can see the details by expanding '>' next to any of the services listed. You can expand the section next to CLI by clicking '>
'
Path: Is the location where the process was launched from within the OS file structure.

Hash: Hash is the value on the process. This is  extra protection, in case a rogue process using a trusted name is launched.

Beahvior analysis: Behavior analysis can be Unknown, Anomalous, or Verified. Analysis for behaviors is displayed for all Processes.

Reputation: Process reputation can be Good, Bad, or Unknown. If bad, investigate further or take immediate action. 

Trust Score and Threat Score: The Trust Score and Threat Score values are provided by a back-end integration with a third-party reputation service for Windows-based services. This integration provides insight into common application processes.For Linux based systems, these scores are derived by integration from various package deployment sites.

Outbound and Inbound Connections: These sections provide information on what ports and IP addresses are being listened to and communicated across.

## Moving to Protected Mode: 
Moving to Protected Mode is a simple proccess. Following the 14 day discovery period there are only a few steps to complete before moving to protected mode. 

## Moving to Protected Mode 

{% include video id="cssrfaDrPpY" provider="youtube" %}

### Procedure for Moving to Protected 

1. Check the behavior chart in the scope dashboard. If more than a couple of behaviors (5+) are being learned over the last couple of days, this scope is not ready for protected mode, let it sit another couple of days. 
2. Check for any malicious processes, integrity alerts, or ML checks. If you see any malicious activity (shown in red), investigate further and take action if needed. 
3. Finally, identify any processes or behaviors that should be deleted/added to blacklist based on internal best practices. 
4. To add the selected scope to the Protected Mode, click the Verify and Protect button at the top of the page. 



<a href="https://vmware-csa-team.github.io/vmware-csa-team/workshop-manual-horizon/"><button>Step Four</button></a>

