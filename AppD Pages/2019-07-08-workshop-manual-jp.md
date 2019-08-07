---
layout: single
title: "Scopes and Services"
permalink: /workshop-manual-jp/
date: 2019-04-02
tags: workshop
classes: wide
author_profile: false
---

After you have finished the deployment of the Appliance, Host, and Guest Modules you can then begin to set up the scopes and services. Please follow the best practices on how to set up scopes and services.

## What is a Scope? 

 A scope is a data center application.

  <img src= "scopedash.png" width= "300" height="600'>

## What is the purpose of a Scope? 

To establish the inteneded state of an application and it's allowed behaviors. 

## What is a service? 

A tier within a scope application which contains desciption, member workloads, rules and behaviors. 

# How to create a Scope and Service

You can manually create a scope and then add a service with members that you have deployed the AppDefense Module to. You can also automate this process through Puppet, Ansible or vRA. Follow the best practices below to create a Scope and Service.

Create a scope (In the AppDefense Manager) : 
1. Click the + icon next to scopes on the left navigation pane
2. insert application name and click create. 

Create a Service within a Scope: 
1. Click add Service. 
2. Select a Service name then select Service type.(ex. app server or web server) 
3. Enter description of this Service and click next.
4. On the Allowed Behavior page, do not add any allowed behaviors right now. System learns the behavior in the Discovery Mode, so you can skip adding any allowed behaviors initially.

Helpful URl's For Scopes and Services: 


