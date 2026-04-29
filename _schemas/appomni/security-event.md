---
description: A security event detected by AppOmni in a SaaS application
layout: schema
name: SecurityEvent
properties_list:
- description: Unique security event identifier
  name: eventId
  type: string
- description: Event severity level
  name: severity
  type: string
- description: Type of security event (anomaly, policy-violation, threat, etc.)
  name: type
  type: string
- description: SaaS application where the event occurred
  name: application
  type: string
- description: Human-readable description of the security event
  name: description
  type: string
- description: Timestamp when the event was detected
  name: detectedAt
  type: string
- description: Event investigation status
  name: status
  type: string
- description: User associated with the event
  name: userId
  type: string
provider_name: AppOmni
provider_slug: appomni
schema_file: json-schema/security-event-schema.json
slug: security-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appomni/main/json-schema/security-event-schema.json\",\n  \"title\": \"SecurityEvent\",\n  \"description\": \"A security event detected by AppOmni in a SaaS application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique security event identifier\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"info\"\n      ],\n      \"description\": \"Event severity level\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of security event (anomaly, policy-violation, threat, etc.)\"\n    },\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"SaaS application where the event occurred\"\n    },\n    \"\
  description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the security event\"\n    },\n    \"detectedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the event was detected\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"investigating\",\n        \"resolved\",\n        \"dismissed\"\n      ],\n      \"description\": \"Event investigation status\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"User associated with the event\"\n    }\n  },\n  \"required\": [\n    \"eventId\",\n    \"severity\",\n    \"type\",\n    \"application\",\n    \"detectedAt\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/json-schema/security-event-schema.json
tags:
- SaaS Security
- Compliance
- Threat Detection
- CASB
- Zero Trust
title: SecurityEvent
---
