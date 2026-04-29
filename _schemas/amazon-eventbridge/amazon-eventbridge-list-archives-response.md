---
description: ListArchivesResponse schema from Amazon EventBridge API
layout: schema
name: ListArchivesResponse
properties_list:
- description: ''
  name: Archives
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-list-archives-response-schema.json
slug: amazon-eventbridge-list-archives-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-archives-response-schema.json\",\n  \"title\": \"ListArchivesResponse\",\n  \"description\": \"ListArchivesResponse schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Archives\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ArchiveName\": {\n            \"type\": \"string\"\n          },\n          \"EventSourceArn\": {\n            \"type\": \"string\"\n          },\n          \"State\": {\n            \"type\": \"string\"\n          },\n          \"RetentionDays\": {\n            \"type\": \"integer\"\n          },\n          \"SizeBytes\": {\n            \"type\": \"integer\"\n          },\n          \"EventCount\": {\n            \"type\": \"integer\"\n    \
  \      },\n          \"CreationTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-archives-response-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: ListArchivesResponse
---
