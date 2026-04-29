---
description: Response from the GetDashboard action
layout: schema
name: GetDashboardResponse
properties_list:
- description: The ARN of the dashboard
  name: dashboardArn
  type: string
- description: The detailed information about the dashboard in JSON format
  name: dashboardBody
  type: string
- description: The name of the dashboard
  name: dashboardName
  type: string
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-get-dashboard-response-schema.json
slug: cloudwatch-get-dashboard-response
source_filename: cloudwatch-get-dashboard-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-get-dashboard-response-schema.json\",\n  \"title\": \"GetDashboardResponse\",\n  \"description\": \"Response from the GetDashboard action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dashboardArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the dashboard\"\n    },\n    \"dashboardBody\": {\n      \"type\": \"string\",\n      \"description\": \"The detailed information about the dashboard in JSON format\"\n    },\n    \"dashboardName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dashboard\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-get-dashboard-response-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: GetDashboardResponse
---
