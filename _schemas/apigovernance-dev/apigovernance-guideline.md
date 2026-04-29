---
description: An API governance guideline or best practice.
layout: schema
name: Guideline
properties_list:
- description: Unique identifier for the guideline.
  name: id
  type: string
- description: Governance category (e.g., Security, Design, Documentation).
  name: category
  type: string
- description: Short title of the guideline.
  name: title
  type: string
- description: Detailed description of the guideline.
  name: description
  type: string
- description: Severity level of violation.
  name: severity
  type: string
- description: Tags categorizing the guideline.
  name: tags
  type: array
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
schema_file: json-schema/apigovernance-guideline-schema.json
slug: apigovernance-guideline
source_filename: apigovernance-guideline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/json-schema/apigovernance-guideline-schema.json\",\n  \"title\": \"Guideline\",\n  \"description\": \"An API governance guideline or best practice.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the guideline.\",\n      \"example\": \"gl-001\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Governance category (e.g., Security, Design, Documentation).\",\n      \"example\": \"Security\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short title of the guideline.\",\n      \"example\": \"Use HTTPS for all API endpoints\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the guideline.\"\n    },\n\
  \    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"info\"\n      ],\n      \"description\": \"Severity level of violation.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags categorizing the guideline.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/json-schema/apigovernance-guideline-schema.json
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
title: Guideline
---
