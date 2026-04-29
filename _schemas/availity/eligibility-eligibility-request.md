---
description: EligibilityRequest schema from Availity API
layout: schema
name: EligibilityRequest
properties_list:
- description: Unique transaction control number (up to 9 characters)
  name: controlNumber
  type: string
- description: ''
  name: provider
  type: object
- description: ''
  name: subscriber
  type: object
- description: ''
  name: dependent
  type: object
- description: ''
  name: payer
  type: object
- description: ''
  name: encounter
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-eligibility-request-schema.json
slug: eligibility-eligibility-request
source_filename: eligibility-eligibility-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-eligibility-request-schema.json\",\n  \"title\": \"EligibilityRequest\",\n  \"description\": \"EligibilityRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"controlNumber\",\n    \"provider\",\n    \"subscriber\",\n    \"payer\"\n  ],\n  \"properties\": {\n    \"controlNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction control number (up to 9 characters)\",\n      \"maxLength\": 9\n    },\n    \"provider\": {\n      \"$ref\": \"#/components/schemas/Provider\"\n    },\n    \"subscriber\": {\n      \"$ref\": \"#/components/schemas/Subscriber\"\n    },\n    \"dependent\": {\n      \"$ref\": \"#/components/schemas/Dependent\"\n    },\n    \"payer\": {\n      \"$ref\": \"#/components/schemas/Payer\"\n    },\n    \"encounter\": {\n \
  \     \"type\": \"object\",\n      \"properties\": {\n        \"serviceTypeCodes\": {\n          \"type\": \"array\",\n          \"description\": \"X12 service type codes (e.g., 30 for Health Benefit Plan Coverage)\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"beginningDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-eligibility-request-schema.json
tags: []
title: EligibilityRequest
---
