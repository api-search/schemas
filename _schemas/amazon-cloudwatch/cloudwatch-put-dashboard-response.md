---
description: Response from the PutDashboard action
layout: schema
name: PutDashboardResponse
properties_list:
- description: Validation messages from the dashboard body
  name: dashboardValidationMessages
  type: array
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-put-dashboard-response-schema.json
slug: cloudwatch-put-dashboard-response
source_filename: cloudwatch-put-dashboard-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-put-dashboard-response-schema.json\",\n  \"title\": \"PutDashboardResponse\",\n  \"description\": \"Response from the PutDashboard action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dashboardValidationMessages\": {\n      \"type\": \"array\",\n      \"description\": \"Validation messages from the dashboard body\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"dataPath\": {\n            \"type\": \"string\",\n            \"description\": \"The data path related to the message\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"A message describing the error or warning\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-put-dashboard-response-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: PutDashboardResponse
---
