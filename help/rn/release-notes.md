---
title: Latest Release
description: This page lists all the new features and improvements for Control Panel
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
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

