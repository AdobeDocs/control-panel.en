---
title: About database monitoring
description: Learn how to monitor workflows on your instances
feature: Control Panel
role: Architect
level: Experienced
---
# Monitor workflows {#monitor-workflows}

## Clean paused and completed workflows

paused completed workflows leave temporary tables that consume space on database
cp allows to clean those tables to free space and therefore improve performances

Technically, executes the clean up technical workflow

process:
1. Database
2. Storage overview details
3. Select temporary resources
4. Clean > confirm
5. In progress, estimated time displays
6. Completion message

## Monitor workflows' parameters 

some options on workflows consume space and lead to performance issues

deactivated by default. CP allows to monitor if some have been activated + to deactivate them

* Keep Result-The option "Keep interim results" of the workflow is checked. This should not be used on production as it could increase drastically database usage.
* Show SQL- The option "Log SQL result" is checked. This could impact platform performances and fill in the log files on the server, which should not be on production.
* Production no supervisor-Workflows with a "Production" flag, but no supervisor operator in the setup to be alerted if the workflow crash.
* A notification/alert, when the temp tables occupy more than 25% of the total allotted DB size. (Example - 500GB of the 2TB).
