---
description: JSON Schema for configuring schema validation pipelines, including validator selection, rule configuration, and output format.
layout: schema
name: Schema Validation Configuration
properties_list:
- description: The schema validator to use for validation.
  name: validator
  type: string
- description: The schema to validate against.
  name: schema
  type: object
- description: The type/specification of the schema being validated.
  name: schemaType
  type: string
- description: The JSON Schema draft version (for JSON Schema validation).
  name: draft
  type: string
- description: Whether to apply strict validation mode rejecting unknown keywords.
  name: strictMode
  type: boolean
- description: Whether to coerce data types to match schema type constraints.
  name: coerceTypes
  type: boolean
- description: Whether to collect all validation errors or stop at the first error.
  name: allErrors
  type: boolean
- description: Output format configuration.
  name: output
  type: object
- description: Custom validation rules (Spectral-style rulesets).
  name: rules
  type: array
provider_name: Schema Validation
provider_slug: schema-validation
schema_file: json-schema/schema-validation-config-schema.json
slug: schema-validation-config
source_filename: schema-validation-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema-validation.apievangelist.com/schema-validation-config-schema.json\",\n  \"title\": \"Schema Validation Configuration\",\n  \"description\": \"JSON Schema for configuring schema validation pipelines, including validator selection, rule configuration, and output format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"validator\": {\n      \"type\": \"string\",\n      \"enum\": [\"ajv\", \"hyperjump\", \"spectral\", \"openapi-schema-validator\", \"blaze\"],\n      \"description\": \"The schema validator to use for validation.\"\n    },\n    \"schema\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL to JSON Schema or OpenAPI spec file\" },\n        { \"type\": \"object\", \"description\": \"Inline JSON Schema object\" }\n      ],\n      \"description\": \"The schema to validate against.\"\n    },\n    \"schemaType\": {\n  \
  \    \"type\": \"string\",\n      \"enum\": [\"json-schema\", \"openapi\", \"asyncapi\", \"graphql\"],\n      \"description\": \"The type/specification of the schema being validated.\"\n    },\n    \"draft\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft-04\", \"draft-06\", \"draft-07\", \"2019-09\", \"2020-12\"],\n      \"description\": \"The JSON Schema draft version (for JSON Schema validation).\"\n    },\n    \"strictMode\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to apply strict validation mode rejecting unknown keywords.\"\n    },\n    \"coerceTypes\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to coerce data types to match schema type constraints.\"\n    },\n    \"allErrors\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to collect all validation errors or stop at the first error.\"\n    },\n    \"output\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Output format configuration.\",\n      \"properties\": {\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\"json\", \"text\", \"junit\", \"sarif\"],\n          \"description\": \"The format for validation output.\"\n        },\n        \"verbosity\": {\n          \"type\": \"string\",\n          \"enum\": [\"error\", \"warn\", \"info\", \"debug\"],\n          \"description\": \"Verbosity level for validation output.\"\n        }\n      }\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"Custom validation rules (Spectral-style rulesets).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ValidationRule\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ValidationRule\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"severity\", \"given\", \"then\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier\
  \ for the rule.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of what the rule validates.\"\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"enum\": [\"error\", \"warn\", \"info\", \"hint\"],\n          \"description\": \"The severity level of a rule violation.\"\n        },\n        \"given\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ],\n          \"description\": \"JSONPath expression(s) identifying the target nodes in the document.\"\n        },\n        \"then\": {\n          \"type\": \"object\",\n          \"description\": \"The function and options to apply to the target nodes.\",\n          \"properties\": {\n            \"function\": {\n              \"type\": \"string\",\n              \"description\": \"The validation function to apply.\"\n         \
  \   },\n            \"functionOptions\": {\n              \"type\": \"object\",\n              \"description\": \"Options passed to the validation function.\",\n              \"additionalProperties\": true\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-validation/refs/heads/main/json-schema/schema-validation-config-schema.json
tags:
- API Governance
- Contract Testing
- JSON Schema
- OpenAPI
- Schema Validation
title: Schema Validation Configuration
---
