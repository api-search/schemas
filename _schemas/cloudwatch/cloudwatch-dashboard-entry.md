---
description: Represents a specific dashboard.
layout: schema
name: DashboardEntry
properties_list:
- description: The name of the dashboard.
  name: DashboardName
  type: string
- description: The Amazon Resource Name (ARN) of the dashboard.
  name: DashboardArn
  type: string
- description: The time stamp of when the dashboard was last modified.
  name: LastModified
  type: string
- description: The size of the dashboard, in bytes.
  name: Size
  type: integer
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-dashboard-entry-schema.json
slug: cloudwatch-dashboard-entry
source_filename: cloudwatch-dashboard-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardEntry\",\n  \"type\": \"object\",\n  \"description\": \"Represents a specific dashboard.\",\n  \"properties\": {\n    \"DashboardName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dashboard.\"\n    },\n    \"DashboardArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the dashboard.\"\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp of when the dashboard was last modified.\"\n    },\n    \"Size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the dashboard, in bytes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-dashboard-entry-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DashboardEntry
---
