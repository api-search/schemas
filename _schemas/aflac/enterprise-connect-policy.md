---
description: A supplemental insurance policy record.
layout: schema
name: Policy
properties_list:
- description: Unique policy identifier.
  name: policy_id
  type: string
- description: Associated enrollment identifier.
  name: enrollment_id
  type: string
- description: Policyholder employee identifier.
  name: employee_id
  type: string
- description: Employer group identifier.
  name: group_id
  type: string
- description: Type of supplemental insurance product.
  name: product_type
  type: string
- description: Policy status.
  name: status
  type: string
- description: Coverage face value amount in USD.
  name: face_value
  type: number
- description: Monthly premium amount in USD.
  name: monthly_premium
  type: number
- description: Policy effective date.
  name: effective_date
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-policy-schema.json
slug: enterprise-connect-policy
source_filename: enterprise-connect-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"A supplemental insurance policy record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy identifier.\",\n      \"example\": \"POL-987654\"\n    },\n    \"enrollment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated enrollment identifier.\",\n      \"example\": \"ENR-500123\"\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Policyholder employee identifier.\",\n      \"example\": \"EMP-789012\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employer group identifier.\",\n      \"example\": \"GRP-123456\"\n    },\n    \"product_type\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Type of supplemental insurance product.\",\n      \"example\": \"accident\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Policy status.\",\n      \"enum\": [\n        \"active\",\n        \"lapsed\",\n        \"terminated\"\n      ],\n      \"example\": \"active\"\n    },\n    \"face_value\": {\n      \"type\": \"number\",\n      \"description\": \"Coverage face value amount in USD.\",\n      \"example\": 50000\n    },\n    \"monthly_premium\": {\n      \"type\": \"number\",\n      \"description\": \"Monthly premium amount in USD.\",\n      \"example\": 18.5\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy effective date.\",\n      \"example\": \"2025-01-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-policy-schema.json
tags: []
title: Policy
---
