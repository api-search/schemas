---
description: A compliance violation found during a check
layout: schema
name: ComplianceViolation
properties_list:
- description: Rule that was violated
  name: rule_id
  type: string
- description: Description of the violation
  name: description
  type: string
- description: Severity of the violation
  name: severity
  type: string
- description: API path where the violation was found
  name: path
  type: string
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-compliance-violation-schema.json
slug: tech-standards-compliance-violation
source_filename: tech-standards-compliance-violation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-compliance-violation-schema.json\",\n  \"title\": \"ComplianceViolation\",\n  \"description\": \"A compliance violation found during a check\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rule_id\": {\n      \"type\": \"string\",\n      \"description\": \"Rule that was violated\",\n      \"example\": \"pag-001\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the violation\",\n      \"example\": \"pageSize parameter missing default value of 20\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity of the violation\",\n      \"enum\": [\n        \"required\",\n        \"recommended\",\n        \"optional\"\n      ],\n      \"example\": \"required\"\n    },\n    \"path\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"API path where the violation was found\",\n      \"example\": \"/policies\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-compliance-violation-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: ComplianceViolation
---
