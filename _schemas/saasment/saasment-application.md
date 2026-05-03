---
description: A SaaS application being monitored by Saasment for security posture management.
layout: schema
name: Saasment Monitored Application
properties_list:
- description: Unique application identifier
  name: id
  type: string
- description: Application display name
  name: name
  type: string
- description: Application category (e.g., Identity & Access Management, Collaboration, CRM)
  name: category
  type: string
- description: Software vendor name
  name: vendor
  type: string
- description: Whether the application integration is active
  name: connected
  type: boolean
- description: Security posture score for this application
  name: posture_score
  type: number
- description: Number of open misconfigurations detected
  name: misconfiguration_count
  type: integer
- description: Timestamp of the last security scan
  name: last_scanned
  type: string
provider_name: Saasment
provider_slug: saasment
schema_file: json-schema/saasment-application-schema.json
slug: saasment-application
source_filename: saasment-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/saasment/main/json-schema/saasment-application-schema.json\",\n  \"title\": \"Saasment Monitored Application\",\n  \"description\": \"A SaaS application being monitored by Saasment for security posture management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique application identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application display name\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Application category (e.g., Identity & Access Management, Collaboration, CRM)\"\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Software vendor name\"\n    },\n    \"connected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application integration\
  \ is active\"\n    },\n    \"posture_score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Security posture score for this application\"\n    },\n    \"misconfiguration_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of open misconfigurations detected\"\n    },\n    \"last_scanned\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last security scan\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"connected\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/json-schema/saasment-application-schema.json
tags:
- SaaS Security
- SSPM
- Cloud Security
- Cost Optimization
- Compliance
- Misconfigurations
title: Saasment Monitored Application
---
