---
description: Result of an eligibility verification check.
layout: schema
name: EligibilityResponse
properties_list:
- description: Whether the employee is eligible for the product.
  name: eligible
  type: boolean
- description: Verified employee identifier.
  name: employee_id
  type: string
- description: Employer group identifier.
  name: group_id
  type: string
- description: Product type checked.
  name: product_type
  type: string
- description: Reason for ineligibility if not eligible.
  name: ineligibility_reason
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-eligibility-response-schema.json
slug: enterprise-connect-eligibility-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-eligibility-response-schema.json\",\n  \"title\": \"EligibilityResponse\",\n  \"description\": \"Result of an eligibility verification check.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eligible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the employee is eligible for the product.\",\n      \"example\": true\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Verified employee identifier.\",\n      \"example\": \"EMP-789012\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employer group identifier.\",\n      \"example\": \"GRP-123456\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Product type checked.\",\n      \"example\": \"accident\"\n    },\n\
  \    \"ineligibility_reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for ineligibility if not eligible.\",\n      \"example\": \"Employee not in an eligible employment class.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-eligibility-response-schema.json
tags: []
title: EligibilityResponse
---
