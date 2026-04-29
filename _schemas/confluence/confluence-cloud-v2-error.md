---
description: Error response from the Confluence API.
layout: schema
name: Error
properties_list:
- description: The HTTP status code.
  name: statusCode
  type: integer
- description: Details about the error.
  name: data
  type: object
- description: A human-readable error message.
  name: message
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-error-schema.json
slug: confluence-cloud-v2-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Error response from the Confluence API.\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the error.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-error-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Error
---
