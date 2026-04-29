---
description: Application schema from openapi
layout: schema
name: Application
properties_list:
- description: The unique identifier of the Amazon Q application.
  name: applicationId
  type: string
- description: The name of the Amazon Q application.
  name: displayName
  type: string
- description: The status of the Amazon Q application.
  name: status
  type: string
- description: The date and time the application was created.
  name: createdAt
  type: string
- description: The date and time the application was last updated.
  name: updatedAt
  type: string
provider_name: Amazon Q
provider_slug: amazon-q
schema_file: json-schema/amazon-q-openapi-application-schema.json
slug: amazon-q-openapi-application
source_filename: amazon-q-openapi-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"Application schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Amazon Q application.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Amazon Q application.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"FAILED\",\n        \"UPDATING\"\n      ],\n      \"description\": \"The status of the Amazon Q application.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  The date and time the application was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the application was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-q/refs/heads/main/json-schema/amazon-q-openapi-application-schema.json
tags:
- Artificial Intelligence
- Assistant
- AWS
- Enterprise
- Generative AI
title: Application
---
