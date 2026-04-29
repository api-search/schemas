---
description: Represents a CloudWatch dashboard
layout: schema
name: Dashboard
properties_list:
- description: The name of the dashboard
  name: dashboardName
  type: string
- description: The ARN of the dashboard
  name: dashboardArn
  type: string
- description: The time stamp of when the dashboard was last modified
  name: lastModified
  type: string
- description: The size of the dashboard in bytes
  name: size
  type: integer
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-dashboard-schema.json
slug: cloudwatch-dashboard
source_filename: cloudwatch-dashboard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-dashboard-schema.json\",\n  \"title\": \"Dashboard\",\n  \"description\": \"Represents a CloudWatch dashboard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dashboardName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dashboard\"\n    },\n    \"dashboardArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the dashboard\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of when the dashboard was last modified\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the dashboard in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-dashboard-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: Dashboard
---
