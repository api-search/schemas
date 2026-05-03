---
description: The webhook event payload delivered by npm hooks when registry changes occur. Each payload is signed with HMAC SHA-256 using the shared secret configured on the hook subscription.
layout: schema
name: npm Hook Event Payload
properties_list:
- description: The type of registry event that occurred.
  name: event
  type: string
- description: The name of the package associated with the event.
  name: name
  type: string
- description: The type of entity that triggered the hook subscription.
  name: type
  type: string
- description: The version of the package associated with the event, if applicable.
  name: version
  type: string
- description: The npm user who owns the hook subscription.
  name: hookOwner
  type: object
- description: Event-specific payload data containing details about what changed.
  name: payload
  type: object
- description: Details about the specific change that occurred.
  name: change
  type: object
- description: The ISO 8601 timestamp of when the event occurred.
  name: time
  type: string
provider_name: npm
provider_slug: npm
schema_file: json-schema/npm-hook-event-schema.json
slug: npm-hook-event
source_filename: npm-hook-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://npmjs.com/schemas/npm/hook-event.json\",\n  \"title\": \"npm Hook Event Payload\",\n  \"description\": \"The webhook event payload delivered by npm hooks when registry changes occur. Each payload is signed with HMAC SHA-256 using the shared secret configured on the hook subscription.\",\n  \"type\": \"object\",\n  \"required\": [\"event\", \"name\", \"type\", \"time\"],\n  \"properties\": {\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The type of registry event that occurred.\",\n      \"enum\": [\n        \"package:change\",\n        \"package:publish\",\n        \"package:unpublish\",\n        \"package:owner\",\n        \"package:dist-tag\",\n        \"package:deprecate\",\n        \"package:star\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the package associated with the event.\"\n    },\n    \"type\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The type of entity that triggered the hook subscription.\",\n      \"enum\": [\"package\", \"scope\", \"owner\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the package associated with the event, if applicable.\"\n    },\n    \"hookOwner\": {\n      \"type\": \"object\",\n      \"description\": \"The npm user who owns the hook subscription.\",\n      \"properties\": {\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The npm username of the hook owner.\"\n        }\n      }\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Event-specific payload data containing details about what changed.\"\n    },\n    \"change\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the specific change that occurred.\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"The affected version, if applicable.\"\n        },\n        \"dist-tag\": {\n          \"type\": \"string\",\n          \"description\": \"The affected dist-tag, if applicable.\"\n        },\n        \"maintainer\": {\n          \"type\": \"string\",\n          \"description\": \"The affected maintainer username, if applicable.\"\n        }\n      }\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp of when the event occurred.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/json-schema/npm-hook-event-schema.json
tags:
- Packages
- JavaScript
- Node.js
- Package Management
- Registry
- Security
title: npm Hook Event Payload
---
