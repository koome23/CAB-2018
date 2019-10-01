# 2018 CAB UX Workshop
![alt text][welcome-cab-members]

The 2018 Customer Advisory Board UX Workshop will be held in Austin on Monday Nov. 12 2018 from 12pm-5pm. This year's UX workshop will focus on the customers **current needs** vs. **future needs** and designing a product to address the current pain points. See below for last year's [pain points](#pain).

Examples of future needs:

* Threats moving to cloud infrastructure (**[Cloud IPS for AWS](#awsf1)**)
* XGen SOC (**[SOC](#soc)**)
* Securing IoT devices (**[IoT](#iotrs)**)

## <a name="pain"></a>Last year's pain points

Below is a list of pain points from 2017 CAB [UX Workshop Report]:

* **Threats In The Wild**:
    * Link active malwares to filters (SPN top threats--**threat intelligence**)
    * Zero day attacks (visibility into **unknown threats**)
    * Attacked vulnerable hosts (eVR **vulnerability** scans)

* **Filter Tuning**:
    * Workflows needed; now manual and resource intensive (IPS policy workflow)
    * Audit trail; what actions were taken for change management (Timeline)
    * Share vertical/industry best practices using Trend's customer data (Healthcare customer ABC enabled filters XYZ we recommend you do the same)

* **Performance Management**:
    * Baseline and benchmark metrics per IPS
    * Central visibility of all appliance stats on SMS
    * Visibility into signature logic/regex rules

### Prototype

**[IPS Policy Workflow]**

Last year's user needs were used to create a [IPS Policy Workflow] prototype (we would love your feedback):

* Automated workflow linking active malware/Zero-day vulnerabilities to filters

* Verification of filter settings are done from within the console

* Audit tracking changes to the filters, showing user comments

## 2018 UX workshop overview

This year's workshop simulates start-up contest inside a company to design a solution addressing the user problems. Like any MVP, the contestants will run through the Research, Product Planning, Design, and Sell phases.

**Agenda**

|Time |Activity |Time |Owner
|---|---|---|---|
|12pm-12:05pm |Opening |5 |Russ |
|12:05pm-12:25pm |Update from last year's CAB workshop |20 |Russ/Michael |
|12:25pm-12:30pm |Workshop overview |5 |Pacha |
|12:30pm-1:00pm |Warm-up game |30 |Pacha |
|1:00pm-2:30pm |Research |90 |Pacha |
|2:30pm-2:40pm |Break |15 | |
|2:40pm-3:25pm |Product planning |45 |Pacha |
|3:25pm-4:15pm |Product design |50 |Pacha |
|4:15pm-4:45pm |Sell |30 |Pacha |
|4:45pm-5:00pm|Closing |15 |Scott |

**[Pre-Workshop]**

Preliminary [materials] in preparation for the workshop. (for Trenders)

**[Research]**

User research/discovery of the current problems and future needs.

**[Product Planning]**

Problem prioritization using an auction process to narrow the scope down to a few specific problems. We'll use these [personas](#personas) to understand our users better.

**[Design]**

Prototype solutions solving the problems in the product planning phase.

**[Sell]**

At this phase, each team will sell their ideas in front of all participants and will be given money to invest. The winning team will be given an award.

### <a name="personas"></a>Personas

The personas we used to understand our users' needs.

**IT System Administrator**

* Monitor network traffic/appliance health status
* Troubleshoot appliances
* Review alerts and generate reports

**Incident Analyst**

* Review-->implement-->distribute
* Write **custom signature**
* Fix vulnerability issues
* Update filters

### Resources

A list of interesting resources...

**[UX Workshop Report]**

Last year's UX workshop report with tons of useful findings summarized and presented to the team by Pacha.

<a name="awsf1"></a>**Cloud IPS for AWS**

Cloud IPS security for AWS.

<a name="iotrs"></a>**IoT**

[Trend Micro IoT Security]

<a name="soc"></a>**SOC**

Trend's initiative for SOC AI enablement unifying siloed data from network, endpoints, email, web gateways, Cloud, data center

[Targeted SOC Use Cases for Effective Incident Detection and Response]

[Maturing Workday's SOC With Splunk]

[How Juniper Networks Manages Incident Response]

[Mitre ATT&CK Matrix]

[welcome-cab-members]: https://www.mhlstudio.net/CAB-2018/images/welcome-cab-members.png "Welcome CAB Members"
[IPS Policy Workflow]: https://sr1l3e.axshare.com/
[storyboard mockups]: https://wiki.jarvis.trendmicro.com/display/TSIM/HIE+Workshop+Storyboard
[Pre-Workshop]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/tree/master/0-Pre-Workshop
[materials]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/tree/master/0-Pre-Workshop/Materials
[Research]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/tree/master/1-Research
[Product Planning]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/tree/master/2-Product%20Planning
[Design]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/tree/master/3-Design
[Sell]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/tree/master/4-Sell
[UX Workshop Report]: https://dsgithub.trendmicro.com/michaellan/CAB-2018/blob/master/Previous-Workshops/CAB%20HIE%20Workshop%20Executive%20Summary.pdf
[Cloud-based IPS]: https://wiki.jarvis.trendmicro.com/display/TPRD/5.2+AWS+F1
[Trend Micro IoT Security]: https://www.trendmicro.com/us/iot-security/
[Targeted SOC Use Cases for Effective Incident Detection and Response]: https://digital-forensics.sans.org/media/Targeted-SOC-Use-Cases-for-effective-Incident-Detection-and-Response-Angelo-Perniola-David-Gray.pdf
[Maturing Workday's SOC With Splunk]: https://conf.splunk.com/files/2016/slides/maturing-workdays-soc-with-splunk.pdf
[How Juniper Networks Manages Incident Response]: https://community.servicenow.com/community?id=community_blog&sys_id=357dbf5edb912380f0612183ca96190f
[Mitre ATT&CK Matrix]: https://attack.mitre.org/matrices/enterprise/
