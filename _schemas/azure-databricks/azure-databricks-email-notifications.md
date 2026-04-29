---
description: ''
layout: schema
name: EmailNotifications
properties_list:
- description: Email addresses to notify when a run starts
  name: on_start
  type: array
- description: Email addresses to notify when a run succeeds
  name: on_success
  type: array
- description: Email addresses to notify when a run fails
  name: on_failure
  type: array
- description: Email addresses to notify when a run exceeds the duration warning threshold
  name: on_duration_warning_threshold_exceeded
  type: array
- description: Do not send alert for skipped runs
  name: no_alert_for_skipped_runs
  type: boolean
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-email-notifications-schema.json
slug: azure-databricks-email-notifications
source_filename: azure-databricks-email-notifications-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailNotifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"on_start\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run starts\"\n    },\n    \"on_success\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run succeeds\"\n    },\n    \"on_failure\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run fails\"\n    },\n    \"on_duration_warning_threshold_exceeded\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses to notify when a run exceeds the duration warning threshold\"\n    },\n    \"no_alert_for_skipped_runs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Do not send alert for skipped runs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-email-notifications-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: EmailNotifications
---
