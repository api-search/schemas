---
description: ''
layout: schema
name: PutDashboardOutput
properties_list:
- description: If the input for PutDashboard was correct, the output includes an empty DashboardValidationMessages array.
  name: DashboardValidationMessages
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-dashboard-output-schema.json
slug: cloudwatch-put-dashboard-output
source_filename: cloudwatch-put-dashboard-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutDashboardOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardValidationMessages\": {\n      \"type\": \"array\",\n      \"description\": \"If the input for PutDashboard was correct, the output includes an empty DashboardValidationMessages array.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-dashboard-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutDashboardOutput
---
