---
description: Request body for checking API compliance
layout: schema
name: ComplianceCheckRequest
properties_list:
- description: URL of the OpenAPI spec to check
  name: openapi_url
  type: string
- description: List of standard IDs to check against
  name: standard_ids
  type: array
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-compliance-check-request-schema.json
slug: tech-standards-compliance-check-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-compliance-check-request-schema.json\",\n  \"title\": \"ComplianceCheckRequest\",\n  \"description\": \"Request body for checking API compliance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"openapi_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the OpenAPI spec to check\",\n      \"example\": \"https://example.com/openapi.yaml\"\n    },\n    \"standard_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of standard IDs to check against\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"std-500001\",\n        \"std-500002\"\n      ]\n    }\n  },\n  \"required\": [\n    \"openapi_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-compliance-check-request-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: ComplianceCheckRequest
---
