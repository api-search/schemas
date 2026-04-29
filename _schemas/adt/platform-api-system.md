---
description: An ADT security system.
layout: schema
name: System
properties_list:
- description: Unique identifier of the system.
  name: id
  type: string
- description: Display name of the system.
  name: name
  type: string
- description: Current arming status.
  name: status
  type: string
- description: Physical address of the protected property.
  name: address
  type: string
- description: Type of security system.
  name: type
  type: string
- description: Timestamp of last status change.
  name: lastModified
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-system-schema.json
slug: platform-api-system
source_filename: platform-api-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-system-schema.json\",\n  \"title\": \"System\",\n  \"description\": \"An ADT security system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the system.\",\n      \"example\": \"sys-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the system.\",\n      \"example\": \"Main House\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current arming status.\",\n      \"enum\": [\n        \"disarmed\",\n        \"armed_away\",\n        \"armed_stay\",\n        \"alarm\",\n        \"arming\"\n      ],\n      \"example\": \"armed_away\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Physical address\
  \ of the protected property.\",\n      \"example\": \"123 Main St, Anytown, CA 90210\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of security system.\",\n      \"enum\": [\n        \"residential\",\n        \"commercial\"\n      ],\n      \"example\": \"residential\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last status change.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-system-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: System
---
