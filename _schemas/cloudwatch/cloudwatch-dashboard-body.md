---
description: The JSON body structure for a CloudWatch dashboard.
layout: schema
name: DashboardBody
properties_list:
- description: An array of dashboard widget objects.
  name: widgets
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-dashboard-body-schema.json
slug: cloudwatch-dashboard-body
source_filename: cloudwatch-dashboard-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardBody\",\n  \"type\": \"object\",\n  \"description\": \"The JSON body structure for a CloudWatch dashboard.\",\n  \"properties\": {\n    \"widgets\": {\n      \"type\": \"array\",\n      \"description\": \"An array of dashboard widget objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-dashboard-body-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DashboardBody
---
