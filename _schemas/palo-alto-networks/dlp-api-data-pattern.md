---
description: DataPattern schema from Palo Alto Networks Enterprise DLP API
layout: schema
name: DataPattern
properties_list:
- description: Unique data pattern identifier.
  name: id
  type: string
- description: Display name of the data pattern.
  name: name
  type: string
- description: Human-readable description of what the pattern detects.
  name: description
  type: string
- description: Whether the pattern is predefined or custom.
  name: type
  type: string
- description: Pattern category (e.g., PII, PCI, HIPAA, Financial).
  name: category
  type: string
- description: Confidence threshold for the pattern.
  name: confidence
  type: string
- description: Detection rule definitions for the pattern.
  name: detection_rules
  type: array
- description: Whether the data pattern is active.
  name: enabled
  type: boolean
- description: Total number of incidents triggered by this pattern.
  name: incident_count
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/dlp-api-data-pattern-schema.json
slug: dlp-api-data-pattern
source_filename: dlp-api-data-pattern-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataPattern\",\n  \"description\": \"DataPattern schema from Palo Alto Networks Enterprise DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-data-pattern-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique data pattern identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the data pattern.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of what the pattern detects.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"predefined\",\n        \"custom\"\n      ],\n      \"description\": \"Whether the pattern is predefined or custom.\"\n    },\n    \"category\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Pattern category (e.g., PII, PCI, HIPAA, Financial).\"\n    },\n    \"confidence\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"high\",\n        \"medium\",\n        \"low\"\n      ],\n      \"description\": \"Confidence threshold for the pattern.\"\n    },\n    \"detection_rules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rule_type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"regex\",\n              \"keyword\",\n              \"dictionary\",\n              \"file_property\"\n            ]\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"proximity\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"Detection rule definitions for the pattern.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the data pattern is active.\"\n    },\n    \"incident_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of incidents triggered by this pattern.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-data-pattern-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataPattern
---
