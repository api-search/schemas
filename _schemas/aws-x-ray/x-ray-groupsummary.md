---
description: ''
layout: schema
name: GroupSummary
properties_list:
- description: ''
  name: GroupName
  type: string
- description: ''
  name: GroupARN
  type: string
- description: ''
  name: FilterExpression
  type: string
- description: ''
  name: InsightsConfiguration
  type: object
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-groupsummary-schema.json
slug: x-ray-groupsummary
source_filename: x-ray-groupsummary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"type\": \"string\"\n    },\n    \"GroupARN\": {\n      \"type\": \"string\"\n    },\n    \"FilterExpression\": {\n      \"type\": \"string\"\n    },\n    \"InsightsConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"InsightsEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"NotificationsEnabled\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-groupsummary-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: GroupSummary
---
