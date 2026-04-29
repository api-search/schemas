---
description: Alarm schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: Alarm
properties_list:
- description: Unique alarm identifier.
  name: id
  type: string
- description: Alarm type identifier.
  name: type
  type: string
- description: Alarm severity level.
  name: severity
  type: string
- description: Site where the alarm was generated.
  name: site_id
  type: string
- description: Name of the site where the alarm was generated.
  name: site_name
  type: string
- description: ION element identifier that generated the alarm.
  name: element_id
  type: string
- description: Human-readable alarm description.
  name: message
  type: string
- description: Whether the alarm has been acknowledged.
  name: acknowledged
  type: boolean
- description: User who acknowledged the alarm.
  name: acknowledged_by
  type: string
- description: Timestamp when the alarm was acknowledged.
  name: acknowledged_at
  type: string
- description: Timestamp when the alarm was raised.
  name: raised_at
  type: string
- description: Timestamp when the alarm was cleared. Null if still active.
  name: cleared_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-alarm-schema.json
slug: prisma-sd-wan-api-alarm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alarm\",\n  \"description\": \"Alarm schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-alarm-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique alarm identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Alarm type identifier.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"major\",\n        \"minor\",\n        \"info\"\n      ],\n      \"description\": \"Alarm severity level.\"\n    },\n    \"site_id\": {\n      \"type\": \"string\",\n      \"description\": \"Site where the alarm was generated.\"\n    },\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Name of the site where the alarm was generated.\"\n    },\n    \"element_id\": {\n      \"type\": \"string\",\n      \"description\": \"ION element identifier that generated the alarm.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable alarm description.\"\n    },\n    \"acknowledged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alarm has been acknowledged.\"\n    },\n    \"acknowledged_by\": {\n      \"type\": \"string\",\n      \"description\": \"User who acknowledged the alarm.\"\n    },\n    \"acknowledged_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alarm was acknowledged.\"\n    },\n    \"raised_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alarm was raised.\"\n    },\n    \"cleared_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"Timestamp when the alarm was cleared. Null if still active.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-alarm-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Alarm
---
