---
description: ''
layout: schema
name: CronSchedule
properties_list:
- description: Quartz cron expression for the schedule. See http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html
  name: quartz_cron_expression
  type: string
- description: Java timezone ID for the schedule
  name: timezone_id
  type: string
- description: Whether the schedule is paused or active
  name: pause_status
  type: string
provider_name: Azure Databricks
provider_slug: microsoft-azure-databricks
schema_file: json-schema/azure-databricks-cron-schedule-schema.json
slug: azure-databricks-cron-schedule
source_filename: azure-databricks-cron-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CronSchedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quartz_cron_expression\": {\n      \"type\": \"string\",\n      \"description\": \"Quartz cron expression for the schedule. See http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html\"\n    },\n    \"timezone_id\": {\n      \"type\": \"string\",\n      \"description\": \"Java timezone ID for the schedule\"\n    },\n    \"pause_status\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the schedule is paused or active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-databricks/refs/heads/main/json-schema/azure-databricks-cron-schedule-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: CronSchedule
---
