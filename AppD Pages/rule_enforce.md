---
layout: single
title: "Rule Enforcement"
permalink: /workshop-manual-pt/
date: 2019-05-20
tags: workshop
classes: wide
author_profile: false
---
## Introduction to Rule Enforcement: 
After the Scope is in Protected Mode, you can still review and edit services associated with the scope.

By default, when  a Scope moves into Protected Mode, the remediation action is set to Alert with automatic enforcement. You can edit rule settings based on the action that you want AppDefense to take in the services tab.

There are four vectors that are used to trigger alert(s) and remediation(s):

- Enforce Outbound Connections: If AppDefense sees a new outbound connection from an allowed process, what do you want it to do?
- Enforce Inbound Connections: If AppDefense sees a new inbound connection from an allowed process, what do you want it to do?
- Enforce Guest OS Integrity: Windows-only. If AppDefense detects that the integrity of your operating system (OS) has been compromised, what do you like it to do?
- Enforce AppDefense Module Integrity: Windows-only. If AppDefense detects the integrity, the AppDefense Module has been compromised (potentially turned off), what do you like it to do?

You cannot set automatic remediation action for the Guest module down alert. Remediation for this action can only be taken manually.


### Quarantine (NSX Only): 
Quarantine is an action of removing a VM from any network, isolating it from the rest of your environment. 

Quarantine is a remediation action that can be enforced by following this procedure: 
1. Select your Scope from Dashboard. 
2. Click on "Services" tab. 
3. Select "Edit service."
4. Click on "Rules" tab. 
5. For your remediation 
action select "Quarantine.

### Block 
Block is a remediation action that will block inbound or outbound network connections, or if using process monitoring block the process before it begins running. 

Block is a remediation action that can be enforced by following this procedure: 
1. Select your Scope from Dashboard. 
2. Click on "Services" tab. 
3. Select "Edit service."
4. Click on "Rules" tab. 
5. For your remediation 
action select "Block and send alert"


### Suspend 

Suspend is a remediation action that will syspend the virtual Machine directly on Vcenter Server. 

Suspend is a remediation action that can be enforced by following this procedure: 
1. Select your Scope from Dashboard. 
2. Click on "Services" tab. 
3. Select "Edit service."
4. Click on "Rules" tab. 
5. For your remediation 
action select "Block and send alert"

### Power Off

Power off is a remediation action that will power down the Virtual machine directly on the vCenter Server.

"Power Off" is a remediation action that can be enforced by following this procedure: 
1. Select your Scope from Dashboard. 
2. Click on "Services" tab. 
3. Select "Edit service."
4. Click on "Rules" tab. 
5. For your remediation 
action select "Power Off"

### Snapshot 

This remediation action will trigger a snapshot of the virtual machine during the time of the incident. 

Snapshot is a remediation action that can be enforced by following this procedure: 
1. Select your Scope from Dashboard. 
2. Click on "Services" tab. 
3. Select "Edit service."
4. Click on "Rules" tab. 
5. For your remediation action select "Snapshot"


