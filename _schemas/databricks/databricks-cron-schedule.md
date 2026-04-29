---
description: ''
layout: schema
name: CronSchedule
properties_list:
- description: A Quartz cron expression describing the schedule. See http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html
  name: quartz_cron_expression
  type: string
- description: A Java timezone ID. The schedule is resolved relative to this timezone.
  name: timezone_id
  type: string
- description: Whether the schedule is paused.
  name: pause_status
  type: string
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-cron-schedule-schema.json
slug: databricks-cron-schedule
source_filename: databricks-cron-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CronSchedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quartz_cron_expression\": {\n      \"type\": \"string\",\n      \"description\": \"A Quartz cron expression describing the schedule. See http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html\"\n    },\n    \"timezone_id\": {\n      \"type\": \"string\",\n      \"description\": \"A Java timezone ID. The schedule is resolved relative to this timezone.\"\n    },\n    \"pause_status\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the schedule is paused.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-cron-schedule-schema.json
tags:
- AI
- Analytics
- Apache Spark
- Big Data
- Clean Rooms
- Cloud Computing
- Data
- Data Analytics
- Data Engineering
- Data Governance
- Delta Lake
- Delta Sharing
- ETL
- Identity Management
- Lakehouse
- Machine Learning
- MLflow
- Model Serving
- Security
- SQL
- Unity Catalog
- Vector Search
- Visualize
title: CronSchedule
---
