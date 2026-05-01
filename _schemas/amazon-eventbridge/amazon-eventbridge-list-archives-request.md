---
description: ListArchivesRequest schema from Amazon EventBridge API
layout: schema
name: ListArchivesRequest
properties_list:
- description: ''
  name: NamePrefix
  type: string
- description: ''
  name: EventSourceArn
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: NextToken
  type: string
- description: ''
  name: Limit
  type: integer
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-list-archives-request-schema.json
slug: amazon-eventbridge-list-archives-request
source_filename: amazon-eventbridge-list-archives-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-archives-request-schema.json\",\n  \"title\": \"ListArchivesRequest\",\n  \"description\": \"ListArchivesRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NamePrefix\": {\n      \"type\": \"string\"\n    },\n    \"EventSourceArn\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    },\n    \"Limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-list-archives-request-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: ListArchivesRequest
---
