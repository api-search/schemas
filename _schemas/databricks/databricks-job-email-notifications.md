---
description: ''
layout: schema
name: JobEmailNotifications
properties_list:
- description: Email addresses to notify when a run starts.
  name: on_start
  type: array
- description: Email addresses to notify when a run succeeds.
  name: on_success
  type: array
- description: Email addresses to notify when a run fails.
  name: on_failure
  type: array
- description: ''
  name: on_duration_warning_threshold_exceeded
  type: array
- description: ''
  name: no_alert_for_skipped_runs
  type: boolean
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-job-email-notifications-schema.json
slug: databricks-job-email-notifications
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobEmailNotifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"on_start\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run starts.\"\n    },\n    \"on_success\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run succeeds.\"\n    },\n    \"on_failure\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run fails.\"\n    },\n    \"on_duration_warning_threshold_exceeded\": {\n      \"type\": \"array\"\n    },\n    \"no_alert_for_skipped_runs\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-job-email-notifications-schema.json
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
title: JobEmailNotifications
---
