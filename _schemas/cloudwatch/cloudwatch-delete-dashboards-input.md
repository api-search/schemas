---
description: ''
layout: schema
name: DeleteDashboardsInput
properties_list:
- description: The dashboards to be deleted. This parameter is required.
  name: DashboardNames
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-delete-dashboards-input-schema.json
slug: cloudwatch-delete-dashboards-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteDashboardsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardNames\": {\n      \"type\": \"array\",\n      \"description\": \"The dashboards to be deleted. This parameter is required.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-delete-dashboards-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DeleteDashboardsInput
---
