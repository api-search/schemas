---
description: Allianz pagination standard definition
layout: schema
name: PaginationGuideline
properties_list:
- description: Unique identifier for the guideline
  name: guideline_id
  type: string
- description: Name of the guideline
  name: name
  type: string
- description: Version of the guideline
  name: version
  type: string
- description: Standardized query parameters for pagination
  name: parameters
  type: array
- description: Standard response headers for pagination
  name: response_headers
  type: array
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schema_file: json-schema/tech-standards-pagination-guideline-schema.json
slug: tech-standards-pagination-guideline
source_filename: tech-standards-pagination-guideline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-pagination-guideline-schema.json\",\n  \"title\": \"PaginationGuideline\",\n  \"description\": \"Allianz pagination standard definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guideline_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the guideline\",\n      \"example\": \"guide-pag-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the guideline\",\n      \"example\": \"Pagination Standard\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the guideline\",\n      \"example\": \"2.1.0\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Standardized query parameters for pagination\",\n      \"items\": {\n\
  \        \"type\": \"object\"\n      }\n    },\n    \"response_headers\": {\n      \"type\": \"array\",\n      \"description\": \"Standard response headers for pagination\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/json-schema/tech-standards-pagination-guideline-schema.json
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
title: PaginationGuideline
---
