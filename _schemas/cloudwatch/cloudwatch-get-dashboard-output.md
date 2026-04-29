---
description: ''
layout: schema
name: GetDashboardOutput
properties_list:
- description: The Amazon Resource Name (ARN) of the dashboard.
  name: DashboardArn
  type: string
- description: The detailed information about the dashboard, including what widgets are included and their location.
  name: DashboardBody
  type: string
- description: The name of the dashboard.
  name: DashboardName
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-get-dashboard-output-schema.json
slug: cloudwatch-get-dashboard-output
source_filename: cloudwatch-get-dashboard-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetDashboardOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the dashboard.\"\n    },\n    \"DashboardBody\": {\n      \"type\": \"string\",\n      \"description\": \"The detailed information about the dashboard, including what widgets are included and their location.\"\n    },\n    \"DashboardName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dashboard.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-get-dashboard-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: GetDashboardOutput
---
