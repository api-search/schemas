---
description: An error or warning for the PutDashboard operation.
layout: schema
name: DashboardValidationMessage
properties_list:
- description: The data path related to the message.
  name: DataPath
  type: string
- description: A message describing the error or warning.
  name: Message
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-dashboard-validation-message-schema.json
slug: cloudwatch-dashboard-validation-message
source_filename: cloudwatch-dashboard-validation-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardValidationMessage\",\n  \"type\": \"object\",\n  \"description\": \"An error or warning for the PutDashboard operation.\",\n  \"properties\": {\n    \"DataPath\": {\n      \"type\": \"string\",\n      \"description\": \"The data path related to the message.\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"A message describing the error or warning.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-dashboard-validation-message-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DashboardValidationMessage
---
