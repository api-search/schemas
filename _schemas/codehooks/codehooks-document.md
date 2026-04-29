---
description: A document in a Codehooks NoSQL collection. Documents are schema-flexible JSON objects with a system-assigned _id.
layout: schema
name: Codehooks Document
properties_list:
- description: Unique document identifier assigned by the system.
  name: _id
  type: string
- description: Timestamp when the document was created.
  name: _createdOn
  type: string
- description: Timestamp when the document was last updated.
  name: _updatedOn
  type: string
provider_name: Codehooks
provider_slug: codehooks
schema_file: json-schema/codehooks-document-schema.json
slug: codehooks-document
source_filename: codehooks-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/json-schema/codehooks-document-schema.json\",\n  \"title\": \"Codehooks Document\",\n  \"description\": \"A document in a Codehooks NoSQL collection. Documents are schema-flexible JSON objects with a system-assigned _id.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique document identifier assigned by the system.\"\n    },\n    \"_createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the document was created.\"\n    },\n    \"_updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the document was last updated.\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"required\": [\"_id\"],\n  \"examples\": [\n    {\n  \
  \    \"_id\": \"64a1b2c3d4e5f60012345678\",\n      \"name\": \"Example document\",\n      \"status\": \"active\",\n      \"_createdOn\": \"2025-06-01T12:00:00.000Z\",\n      \"_updatedOn\": \"2025-06-01T12:00:00.000Z\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/json-schema/codehooks-document-schema.json
tags:
- Backend
- Database
- Events
- Hooks
- JavaScript
- NoSQL
- Queues
- Serverless
- Webhooks
- Workers
- Workflows
title: Codehooks Document
---
