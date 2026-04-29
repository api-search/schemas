---
description: CreateArchiveRequest schema from Amazon EventBridge API
layout: schema
name: CreateArchiveRequest
properties_list:
- description: ''
  name: ArchiveName
  type: string
- description: ''
  name: EventSourceArn
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: EventPattern
  type: string
- description: ''
  name: RetentionDays
  type: integer
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-create-archive-request-schema.json
slug: amazon-eventbridge-create-archive-request
source_filename: amazon-eventbridge-create-archive-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-create-archive-request-schema.json\",\n  \"title\": \"CreateArchiveRequest\",\n  \"description\": \"CreateArchiveRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArchiveName\": {\n      \"type\": \"string\"\n    },\n    \"EventSourceArn\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"EventPattern\": {\n      \"type\": \"string\"\n    },\n    \"RetentionDays\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"ArchiveName\",\n    \"EventSourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-create-archive-request-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: CreateArchiveRequest
---
