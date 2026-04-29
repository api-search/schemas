---
description: An individual rule within a technology standard
layout: schema
name: StandardRule
properties_list:
- description: Unique identifier for the rule
  name: rule_id
  type: string
- description: Human-readable description of the rule
  name: description
  type: string
- description: Severity level of the rule
  name: severity
  type: string
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-standard-rule-schema.json
slug: tech-standards-standard-rule
source_filename: tech-standards-standard-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-standard-rule-schema.json\",\n  \"title\": \"StandardRule\",\n  \"description\": \"An individual rule within a technology standard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rule_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the rule\",\n      \"example\": \"pag-001\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the rule\",\n      \"example\": \"pageSize parameter must default to 20\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the rule\",\n      \"enum\": [\n        \"required\",\n        \"recommended\",\n        \"optional\"\n      ],\n      \"example\": \"required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-standard-rule-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: StandardRule
---
