---
description: A leave request in absentify.
layout: schema
name: Request
properties_list:
- description: Unique identifier of the request.
  name: id
  type: string
- description: Start date of the request.
  name: start
  type: string
- description: Time of day when the leave starts.
  name: start_at
  type: string
- description: End date of the request.
  name: end
  type: string
- description: Time of day when the leave ends.
  name: end_at
  type: string
- description: Current status of the request.
  name: status
  type: string
- description: Reason for the leave request.
  name: reason
  type: string
- description: Duration of the leave.
  name: duration
  type: number
- description: Timestamp when the request was created.
  name: createdAt
  type: string
- description: Timestamp when the request was last updated.
  name: updatedAt
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-request-schema.json
slug: absentify-request
source_filename: absentify-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-request-schema.json\",\n  \"title\": \"Request\",\n  \"description\": \"A leave request in absentify.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the request.\",\n      \"example\": \"500456\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the request.\",\n      \"example\": \"2025-06-01\"\n    },\n    \"start_at\": {\n      \"type\": \"string\",\n      \"description\": \"Time of day when the leave starts.\",\n      \"example\": \"morning\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the request.\"\
  ,\n      \"example\": \"2025-06-05\"\n    },\n    \"end_at\": {\n      \"type\": \"string\",\n      \"description\": \"Time of day when the leave ends.\",\n      \"example\": \"afternoon\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the request.\",\n      \"example\": \"APPROVED\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the leave request.\",\n      \"example\": \"Annual vacation\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Duration of the leave.\",\n      \"example\": 5\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the request was created.\",\n      \"example\": \"2025-05-15T10:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the request was last updated.\",\n\
  \      \"example\": \"2025-05-16T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-request-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: Request
---
