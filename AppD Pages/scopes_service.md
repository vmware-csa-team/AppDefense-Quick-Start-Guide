---
layout: single
title: "Scopes and Services"
permalink: /workshop-manual-jp/
date: 2019-04-02
tags: workshop
classes: wide
author_profile: false
---

After you have finished the deployment of the Appliance, Host, and Guest Modules you can then begin to set up scopes and services. Please follow the best practices on how to set up scopes and services.

## Scope and Service creation tutorial
{% include video id="ZCql21viGDY" provider="youtube" %}

## What is a Scope? 

 A scope is a data center application.

## What is the purpose of a Scope? 

The purpose of a scope is to establish the inteneded state of an application and it's allowed behaviors. 

## What is a Service? 

A service is a tier within a data center application (i.e web,app,DB,etc).In AppDefense a service should contain homogenous members (VMs), and where the verified behavior list and rules will be located for learned processes. 

# How to create a Scope and Service

You can manually create a scope and then add a service with members that you have deployed the AppDefense Module to. You can also automate this process through Puppet, Ansible or vRA. Follow the best practices below to create a Scope and Service.

Create a scope (In the AppDefense Manager) : 
1. Click the + icon next to scopes on the left navigation pane.
2. insert application name and click create. 

Create a Service within a Scope: 
1. Click add Service. 
2. Select a Service name then select Service type.(ex. app server or web server) 
3. Enter description of this Service and click next (optional).
4. On the Allowed Behavior page, do not add any allowed behaviors right now. System learns the behavior in the Discovery Mode, so you can skip adding any allowed behaviors initially.


    <a href="https://vmware-csa-team.github.io/vmware-csa-team/workshop-manual/"><button>Step Three</button></a>
     

