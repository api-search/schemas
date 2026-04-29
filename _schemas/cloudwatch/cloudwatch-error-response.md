---
description: Standard error response from CloudWatch API.
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: Error
  type: object
- description: The unique request ID.
  name: RequestId
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-error-response-schema.json
slug: cloudwatch-error-response
source_filename: cloudwatch-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response from CloudWatch API.\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"object\"\n    },\n    \"RequestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique request ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-error-response-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ErrorResponse
---
