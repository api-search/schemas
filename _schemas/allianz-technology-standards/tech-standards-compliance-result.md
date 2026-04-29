---
description: Result of a compliance check
layout: schema
name: ComplianceResult
properties_list:
- description: Unique identifier for the compliance check
  name: check_id
  type: string
- description: Status of the compliance check
  name: status
  type: string
- description: Number of rules that passed
  name: passed
  type: integer
- description: Number of rules that failed
  name: failed
  type: integer
- description: Number of warnings found
  name: warnings
  type: integer
- description: List of compliance violations found
  name: violations
  type: array
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-compliance-result-schema.json
slug: tech-standards-compliance-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-compliance-result-schema.json\",\n  \"title\": \"ComplianceResult\",\n  \"description\": \"Result of a compliance check\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"check_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the compliance check\",\n      \"example\": \"chk-500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the compliance check\",\n      \"enum\": [\n        \"pending\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"example\": \"completed\"\n    },\n    \"passed\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rules that passed\",\n      \"example\": 18\n    },\n    \"failed\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Number of rules that failed\",\n      \"example\": 3\n    },\n    \"warnings\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of warnings found\",\n      \"example\": 5\n    },\n    \"violations\": {\n      \"type\": \"array\",\n      \"description\": \"List of compliance violations found\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ComplianceViolation\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-compliance-result-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: ComplianceResult
---
