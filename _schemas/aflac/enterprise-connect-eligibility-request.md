---
description: Request payload for eligibility verification.
layout: schema
name: EligibilityRequest
properties_list:
- description: Employee identifier to verify.
  name: employee_id
  type: string
- description: Employer group identifier.
  name: group_id
  type: string
- description: Supplemental insurance product to check eligibility for.
  name: product_type
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-eligibility-request-schema.json
slug: enterprise-connect-eligibility-request
source_filename: enterprise-connect-eligibility-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-eligibility-request-schema.json\",\n  \"title\": \"EligibilityRequest\",\n  \"description\": \"Request payload for eligibility verification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee identifier to verify.\",\n      \"example\": \"EMP-789012\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employer group identifier.\",\n      \"example\": \"GRP-123456\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Supplemental insurance product to check eligibility for.\",\n      \"example\": \"accident\"\n    }\n  },\n  \"required\": [\n    \"employee_id\",\n    \"group_id\",\n    \"product_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-eligibility-request-schema.json
tags: []
title: EligibilityRequest
---
