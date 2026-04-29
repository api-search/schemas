---
description: ''
layout: schema
name: ListDashboardsInput
properties_list:
- description: If you specify this parameter, only the dashboards with names starting with the specified string are listed.
  name: DashboardNamePrefix
  type: string
- description: The token returned by a previous call to indicate there is more data available.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-dashboards-input-schema.json
slug: cloudwatch-list-dashboards-input
source_filename: cloudwatch-list-dashboards-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListDashboardsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardNamePrefix\": {\n      \"type\": \"string\",\n      \"description\": \"If you specify this parameter, only the dashboards with names starting with the specified string are listed.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token returned by a previous call to indicate there is more data available.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-dashboards-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListDashboardsInput
---
