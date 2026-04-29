---
description: A key-value entry in the Codehooks key-value store, supporting string or object values with optional TTL-based expiration.
layout: schema
name: Codehooks Key-Value Entry
properties_list:
- description: The unique key identifier for the stored value.
  name: key
  type: string
- description: The stored value, which can be a string, number, or JSON object.
  name: value
  type: object
- description: Time-to-live in milliseconds for automatic expiration of the key-value pair.
  name: ttl
  type: integer
provider_name: Codehooks
provider_slug: codehooks
schema_file: json-schema/codehooks-key-value-schema.json
slug: codehooks-key-value
source_filename: codehooks-key-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/json-schema/codehooks-key-value-schema.json\",\n  \"title\": \"Codehooks Key-Value Entry\",\n  \"description\": \"A key-value entry in the Codehooks key-value store, supporting string or object values with optional TTL-based expiration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key identifier for the stored value.\"\n    },\n    \"value\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      ],\n      \"description\": \"The stored value, which can be a string, number, or JSON object.\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Time-to-live in milliseconds for automatic expiration of the key-value pair.\",\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\"key\", \"value\"],\n  \"additionalProperties\": false,\n  \"examples\": [\n    {\n      \"key\": \"session:abc123\",\n      \"value\": \"authenticated\",\n      \"ttl\": 3600000\n    },\n    {\n      \"key\": \"config:feature-flags\",\n      \"value\": {\n        \"darkMode\": true,\n        \"betaAccess\": false\n      }\n    },\n    {\n      \"key\": \"counter:page-views\",\n      \"value\": 42\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/codehooks/refs/heads/main/json-schema/codehooks-key-value-schema.json
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
title: Codehooks Key-Value Entry
---
