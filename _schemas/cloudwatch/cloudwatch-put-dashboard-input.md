---
description: ''
layout: schema
name: PutDashboardInput
properties_list:
- description: The name of the dashboard. If a dashboard with this name already exists, this call modifies that dashboard.
  name: DashboardName
  type: string
- description: The detailed information about the dashboard in JSON format, including the widgets to include and their location on the dashboard. For more information about the syntax, see Dashboard Body Structure a
  name: DashboardBody
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-dashboard-input-schema.json
slug: cloudwatch-put-dashboard-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutDashboardInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dashboard. If a dashboard with this name already exists, this call modifies that dashboard.\"\n    },\n    \"DashboardBody\": {\n      \"type\": \"string\",\n      \"description\": \"The detailed information about the dashboard in JSON format, including the widgets to include and their location on the dashboard. For more information about the syntax, see Dashboard Body Structure and Syntax.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-dashboard-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutDashboardInput
---
