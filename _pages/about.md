---
layout: single
permalink: /about/
title: "Frequently asked questions"
date: 2018-06-02
tags: about
classes: wide
---

Here you will find questions that are frequently asked about AppDefense. 


### How to get support from Appdefense?

There are two ways to get support with VMware AppDefense:

1. Chatting in the AppDefense manager with a technical engineer.
2. Logging a ticket through ‘My VMware’ portal (traditional support method).

For more information on this topic please visit our community blog page:
[How do you get support for Vmware AppDefense?](https://communities.vmware.com/thread/616075){:target="_blank"} 



### How long does it take to install? 

VMware AppDefense should take no longer than 4-5 weeks to get to a protected state. For the majority of this time, the application will be in Discovery Mode (1-3 weeks), requiring no user action. 

For more information on this topic please visit our community blog page:
[How long does AppDefense take to install?](https://communities.vmware.com/message/2872636#2872636){:target="_blank"} 

### How do I Install AppDefense? 

Physical Deployment

1. First, deploy the appliance into the vCenter that you will deploy AppDefense to (one per vCenter).
2. After the appliance is deployed, then deploy the host module through the AppDefense Manager.
3. Be sure that vib is installed on all hosts that will have VMs with AppDefense on them (there will be no downtime installing on the host(s).
4. Finally, install to the guest through VMtools. (enable guest integrity and plan accordingly as this will take a reboot of the guest).

For further steps please visit our our community blog page:  
[How do I Install Appdefense?](https://communities.vmware.com/thread/613569){:target="_blank"} 


### How should I setup Scopes and Services? 

Scope and Service Creation based on tiers within an application: 

1. From the dashboard in the AppDefense manager click create Scope and name the Scope after your data center application.
2. From here, select “add service” and name the Service after the tier within your data center application. (If you do not see your service type listed you can select “other”- this is not an essential part of the service creation)
3. Next, you will be able to select members. (note that members must be homogenous, i.e. do not put an App server and DB server in the same service.)
4. Add behaviors if you have them if not this step will be done in the Discovery phase.

For further steps please visit our community blog page: 
[How Should I setup Scope and Services?](https://communities.vmware.com/thread/614669){:target="_blank"} 


### What happens when Discovery Mode ends? 

After 2-3 weeks the learning phase of Discovery Mode will be complete and your scope will be ready to move into Protected Mode. Remember that in Protected Mode any deviations from your verified behavior list will trigger an alert, an event, and if rules have been set up they will be enforced.

For further steps please visit our community blog page: 
[What happens when Discovery Mode ends?](https://communities.vmware.com/thread/615819){:target="_blank"}








