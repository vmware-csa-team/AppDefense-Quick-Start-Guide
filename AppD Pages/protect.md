---
layout: single
title: "Protected Mode"
permalink: /workshop-manual-horizon/
date: 2019-03-19
tags: workshop
classes: wide
author_profile: false
---
## What is Protected Mode? 
In Protected Mode, application behavior is locked down, and rules are applied.

### What happens when I move my Scope into Protected Mode? 
When a scope moves into Protected Mode, all application behavior will be locked down, and if rules and remediation actions are setup they will be enforced (the default rule is alert only-no action will be taken). The armor is applied , and your application is now safe in Protected Mode.

## Types of Deviations
When a scope enters Protected Mode, the process and behavior deviations from the verified behavior list will go through our classification engine. The results will be one of the following: Critical Alerts, Serious Alerts, Minor Event, Info Event, Provisioning Events, and System Updates. 

The deviations from the verified behavior list consist of the following: 

- Process-driven events = Process Monitoring, Inbound connections, Outbound connections. 
- System integrity-driven events = Appdefense module Integrity, Guest OS Integrity
- Management Driven Events= Management Alert, Guest module down 

## Alerts 
What are Alerts? 
- AppDefense learns the behaviors (discovery mode) and sends alerts based on the rule settings.
- Any deviation from the known good state triggers an event or alert. The deviation can be due to process characteristics, process behavior,the integrity of the Operating System (OS), or AppDefense module tampering. Alerts are the most critical deviations based on social assurance and threat scores.
## Alert Classification

{% include video id="QbmfQBalTGw" provider="youtube" %}

AppDefense classifies alerts based on their threat level.In the AppDefense Manager,ckick the "alerts" button located on the left navigation pane. The alerts are grouped based on the process name. Critical and Serious Alerts are only displayed in the Alerts page. All Alerts should be investigated and when necessary, take immediate action. 

Example of Alerts:

- Guest Module Down
- Guest Integrity (something has changed in the Kernal)
- Low social assurance score on process
- Blacklisted process

## Events
AppDefense generates different types and subtypes (categories) of alerts and events, with different severity levels. The Alerts page displays only critical and serious process deviations, whereas events display minor deviations. 

Example of Events (minor, info, provisioning, updates):

- known process new behavior (Trusted process reaches out to a new IP)
- Microsoft application update
- New scope provisioned in AppDefense


## Blacklist and Whitelist 
- Blacklist: is the explicit listing of processes that are not allowed in an org, when added to the Blacklist a process will be removed from every service in every scope.  
- Whitelist: is an explicit listing of processes that are allowed, once added to the Whitelist a process will be added to every service within every scope.  This can be applied in the service or in the "manage process" tab. 


<a href="https://vmware-csa-team.github.io/vmware-csa-team/workshop-manual-pt/"><button>Optional Rule Enforcement Step</button></a>

