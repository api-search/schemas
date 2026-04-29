---
description: ''
layout: schema
name: WebhookNotifications
properties_list:
- description: ''
  name: on_start
  type: array
- description: ''
  name: on_success
  type: array
- description: ''
  name: on_failure
  type: array
- description: ''
  name: on_duration_warning_threshold_exceeded
  type: array
provider_name: Databricks
provider_slug: databricks
schema_file: json-schema/databricks-webhook-notifications-schema.json
slug: databricks-webhook-notifications
source_filename: databricks-webhook-notifications-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebhookNotifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"on_start\": {\n      \"type\": \"array\"\n    },\n    \"on_success\": {\n      \"type\": \"array\"\n    },\n    \"on_failure\": {\n      \"type\": \"array\"\n    },\n    \"on_duration_warning_threshold_exceeded\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/databricks/refs/heads/main/json-schema/databricks-webhook-notifications-schema.json
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
title: WebhookNotifications
---
