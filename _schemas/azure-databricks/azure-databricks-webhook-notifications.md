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
provider_name: Azure Databricks
provider_slug: azure-databricks
schema_file: json-schema/azure-databricks-webhook-notifications-schema.json
slug: azure-databricks-webhook-notifications
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebhookNotifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"on_start\": {\n      \"type\": \"array\"\n    },\n    \"on_success\": {\n      \"type\": \"array\"\n    },\n    \"on_failure\": {\n      \"type\": \"array\"\n    },\n    \"on_duration_warning_threshold_exceeded\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/json-schema/azure-databricks-webhook-notifications-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
title: WebhookNotifications
---
