---
description: List of ADT security systems.
layout: schema
name: SystemList
properties_list:
- description: Array of security systems.
  name: systems
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-system-list-schema.json
slug: platform-api-system-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-system-list-schema.json\",\n  \"title\": \"SystemList\",\n  \"description\": \"List of ADT security systems.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"systems\": {\n      \"type\": \"array\",\n      \"description\": \"Array of security systems.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An ADT security system.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the system.\",\n            \"example\": \"sys-001\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the system.\",\n            \"example\": \"Main House\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n   \
  \         \"description\": \"Current arming status.\",\n            \"enum\": [\n              \"disarmed\",\n              \"armed_away\",\n              \"armed_stay\",\n              \"alarm\",\n              \"arming\"\n            ],\n            \"example\": \"armed_away\"\n          },\n          \"address\": {\n            \"type\": \"string\",\n            \"description\": \"Physical address of the protected property.\",\n            \"example\": \"123 Main St, Anytown, CA 90210\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of security system.\",\n            \"enum\": [\n              \"residential\",\n              \"commercial\"\n            ],\n            \"example\": \"residential\"\n          },\n          \"lastModified\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp of last status change.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\
  \n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-system-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: SystemList
---
