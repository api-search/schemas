---
description: Coverage schema from Availity API
layout: schema
name: Coverage
properties_list:
- description: ''
  name: serviceTypeCodes
  type: array
- description: ''
  name: serviceTypeNames
  type: array
- description: ''
  name: insuranceType
  type: string
- description: ''
  name: planCoverage
  type: string
- description: ''
  name: coverageStatus
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: benefits
  type: array
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-coverage-schema.json
slug: eligibility-coverage
source_filename: eligibility-coverage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-coverage-schema.json\",\n  \"title\": \"Coverage\",\n  \"description\": \"Coverage schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceTypeCodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"serviceTypeNames\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"insuranceType\": {\n      \"type\": \"string\"\n    },\n    \"planCoverage\": {\n      \"type\": \"string\"\n    },\n    \"coverageStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Inactive\",\n        \"Cancelled\"\n      ]\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"expirationDate\": {\n \
  \     \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"benefits\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Benefit\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-coverage-schema.json
tags: []
title: Coverage
---
