---
description: Schema for the output of the Redocly CLI lint command.
layout: schema
name: Redocly Lint Result
properties_list:
- description: Aggregate counts of lint findings.
  name: totals
  type: object
- description: Per-file finding counts.
  name: fileTotals
  type: object
- description: List of lint violations.
  name: problems
  type: array
provider_name: Redocly
provider_slug: redocly
schema_file: json-schema/redocly-lint-result-schema.json
slug: redocly-lint-result
source_filename: redocly-lint-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redocly.com/schemas/lint-result.json\",\n  \"title\": \"Redocly Lint Result\",\n  \"description\": \"Schema for the output of the Redocly CLI lint command.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totals\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregate counts of lint findings.\",\n      \"properties\": {\n        \"errors\": { \"type\": \"integer\", \"description\": \"Number of error-severity violations.\" },\n        \"warnings\": { \"type\": \"integer\", \"description\": \"Number of warning-severity violations.\" },\n        \"ignored\": { \"type\": \"integer\", \"description\": \"Number of suppressed violations.\" }\n      }\n    },\n    \"fileTotals\": {\n      \"type\": \"object\",\n      \"description\": \"Per-file finding counts.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"errors\"\
  : { \"type\": \"integer\" },\n          \"warnings\": { \"type\": \"integer\" },\n          \"ignored\": { \"type\": \"integer\" }\n        }\n      }\n    },\n    \"problems\": {\n      \"type\": \"array\",\n      \"description\": \"List of lint violations.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LintProblem\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"LintProblem\": {\n      \"type\": \"object\",\n      \"required\": [\"message\", \"severity\", \"ruleId\"],\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the violation.\"\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"enum\": [\"error\", \"warn\"],\n          \"description\": \"Severity level of the violation.\"\n        },\n        \"ruleId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the rule that triggered the violation.\"\n        },\n        \"location\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Locations in the OpenAPI document where the violation occurred.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"source\": { \"type\": \"string\", \"description\": \"File path.\" },\n              \"pointer\": { \"type\": \"string\", \"description\": \"JSON Pointer to the violating element.\" },\n              \"line\": { \"type\": \"integer\", \"description\": \"Line number.\" },\n              \"col\": { \"type\": \"integer\", \"description\": \"Column number.\" }\n            }\n          }\n        },\n        \"suggest\": {\n          \"type\": \"array\",\n          \"description\": \"Suggested fixes.\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/json-schema/redocly-lint-result-schema.json
tags:
- API Catalog
- API Documentation
- Developer Portal
- Governance
- Linting
- OpenAPI
title: Redocly Lint Result
---
