---
description: A security misconfiguration detected by Saasment SSPM across monitored SaaS applications.
layout: schema
name: Saasment Misconfiguration
properties_list:
- description: Unique identifier for the misconfiguration
  name: id
  type: string
- description: Short descriptive title of the misconfiguration
  name: title
  type: string
- description: Detailed description of the security issue
  name: description
  type: string
- description: Risk severity level of the misconfiguration
  name: severity
  type: string
- description: Security category (e.g., Identity Security, Access Control, Data Protection)
  name: category
  type: string
- description: ID of the SaaS application where the misconfiguration was detected
  name: app_id
  type: string
- description: Name of the SaaS application
  name: app_name
  type: string
- description: Current remediation status
  name: status
  type: string
- description: Step-by-step remediation guidance
  name: remediation
  type: string
- description: Timestamp when the misconfiguration was first detected
  name: detected_at
  type: string
- description: Timestamp of last status update
  name: updated_at
  type: string
provider_name: Saasment
provider_slug: saasment
schema_file: json-schema/saasment-misconfiguration-schema.json
slug: saasment-misconfiguration
source_filename: saasment-misconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/saasment/main/json-schema/saasment-misconfiguration-schema.json\",\n  \"title\": \"Saasment Misconfiguration\",\n  \"description\": \"A security misconfiguration detected by Saasment SSPM across monitored SaaS applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the misconfiguration\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short descriptive title of the misconfiguration\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the security issue\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"critical\", \"high\", \"medium\", \"low\", \"info\"],\n      \"description\": \"Risk severity level of the misconfiguration\"\n\
  \    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Security category (e.g., Identity Security, Access Control, Data Protection)\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the SaaS application where the misconfiguration was detected\"\n    },\n    \"app_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SaaS application\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"open\", \"in_progress\", \"resolved\", \"accepted\"],\n      \"description\": \"Current remediation status\"\n    },\n    \"remediation\": {\n      \"type\": \"string\",\n      \"description\": \"Step-by-step remediation guidance\"\n    },\n    \"detected_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the misconfiguration was first detected\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp of last status update\"\n    }\n  },\n  \"required\": [\"id\", \"title\", \"severity\", \"category\", \"app_id\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/json-schema/saasment-misconfiguration-schema.json
tags:
- SaaS Security
- SSPM
- Cloud Security
- Cost Optimization
- Compliance
- Misconfigurations
title: Saasment Misconfiguration
---
