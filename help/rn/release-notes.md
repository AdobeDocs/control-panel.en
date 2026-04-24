---
title: Latest Release
description: This page lists all the new features and improvements for Control Panel
feature: Control Panel, Release Notes
role: Admin
level: Experienced
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
TQID: https://experienceleague.adobe.com/Q1kU0q1e-a-H0LvAyK-5yYhfrUpGco1hVHWUsz-syhY
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---
# Latest Release {#control-panel-releases}

This page lists the new features and improvements for Control Panel.

## October 2023 {#october-2023}

**User interface**

* Control Panel is now available in additional languages. [Learn more](../discover/using/discovering-the-interface.md#supported-languages-languages)

**Active profiles monitoring**

* You can now monitor the number of active profiles you are entitled to for your organization, and the total count of profiles used in your organization within all instances, if you are using multiple instances. [Learn more](../performance-monitoring/using/active-profiles-monitoring.md)

**DMARC records**

* Multiple email addresses can now receive aggregate report and failure report emails. [Learn more](../subdomains-certificates/using/dmarc.md)
* Changes have been made if both DMARC and BIMI records exist for a subdomain:

    * DMARC records cannot deleted. If you want to delete one, you need to delete the BIMI record first.
    * DMARC records can be edited, but the policy downgrade to "None" is not allowed and its percentage value must be 100.

