---
description: A cron-based schedule for automatic workflow execution in Apache DolphinScheduler.
layout: schema
name: Schedule
properties_list:
- description: Schedule ID.
  name: id
  type: integer
- description: Workflow definition code to schedule.
  name: processDefinitionCode
  type: integer
- description: Cron expression for the schedule.
  name: crontab
  type: string
- description: Schedule start datetime.
  name: startTime
  type: string
- description: Schedule end datetime.
  name: endTime
  type: string
- description: Timezone for cron evaluation.
  name: timezoneId
  type: string
- description: Strategy on schedule failure.
  name: failureStrategy
  type: string
- description: When to send alerts.
  name: warningType
  type: string
- description: Whether this schedule is active.
  name: releaseState
  type: string
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-schedule-schema.json
slug: apache-dolphinscheduler-schedule
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: Schedule
---
