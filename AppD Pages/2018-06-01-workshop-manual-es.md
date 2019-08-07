---
layout: single
title: "Deploying AppDefense"
permalink: /workshop-manual-es/
date: 2018-09-08
tags: workshop
classes: wide
author_profile: false
---
## Deployment Timeline

AppDefense takes between 4-6 weeks to fully deploy and operationalize. Below is an overview of the weekly deployment schedule once all pre-requistes are met: 

### Week One:
Deploy the Appdefense Appliance, Host,  and Guest Modules. (This step)
Set up scopes and Services

### Week Two-Three:
Once Scopes and Services are set up discovery will begin.
No user action for this period of time

### Week Four-Five:
Check the Scope Dashboard to see if the number of behaviors learned over time has tapered off
Move to protected mode
Integrate with internal SIEM

Beyond: 
Identify and implement desired rules for service(s)

## AppDefense Deployment Demo 
{% include video id="D2nMRzmJXF0" provider="youtube" %}

## Deployment Procedure 
1. Deploy the OVA: 
- Networking requirements: Appliance IP,gateway,fully qualified domain name,search path, domain IP, netmask
- Root password cannot be recovered.
- Root and Admin password must be at least 8 characters with complexity requirements. 
2. Register appliance
- HTTPS:// < Appliance IP >
- You will need SSO credentials to register the appliance.
3. Deploy host from AppDefense Manager
- VIB only install, does not require reboot. 
- This needs to be done with every host that will have AppDefense enabled VMs
4. Deploy Guest Module (through VMtools)
you will need version 10.3.2 or higher of VMtools
- Please plan for a reboot with the guest module install
- Check some of our blogs for scripting tips to deploy to many VMs
- Enable guest integrity from the AppDefense Manager 
- Deploy the guest module

### Helpful URL's

Find helpful links to documentation and videos related to deployment below

Appdefense Deployment cycle explained by Paige Clapper: <https://www.youtube.com/watch?v=PYH9Cdg6F9Q&t=1s>

Deployment Tutorial:  <https://www.youtube.com/watch?v=D2nMRzmJXF0&t=40s>

