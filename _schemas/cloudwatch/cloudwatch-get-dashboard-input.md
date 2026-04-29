---
description: ''
layout: schema
name: GetDashboardInput
properties_list:
- description: The name of the dashboard to be described.
  name: DashboardName
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-get-dashboard-input-schema.json
slug: cloudwatch-get-dashboard-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetDashboardInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dashboard to be described.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-get-dashboard-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: GetDashboardInput
---
