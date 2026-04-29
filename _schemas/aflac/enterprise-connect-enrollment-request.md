---
description: Request payload for creating or updating an enrollment.
layout: schema
name: EnrollmentRequest
properties_list:
- description: Employee identifier.
  name: employee_id
  type: string
- description: Employer group identifier.
  name: group_id
  type: string
- description: Type of supplemental insurance product to enroll in.
  name: product_type
  type: string
- description: Coverage level for the enrollment.
  name: coverage_level
  type: string
- description: Requested effective date for coverage.
  name: effective_date
  type: string
- description: List of dependents to include in family coverage.
  name: dependents
  type: array
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-enrollment-request-schema.json
slug: enterprise-connect-enrollment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-enrollment-request-schema.json\",\n  \"title\": \"EnrollmentRequest\",\n  \"description\": \"Request payload for creating or updating an enrollment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee identifier.\",\n      \"example\": \"EMP-789012\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employer group identifier.\",\n      \"example\": \"GRP-123456\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of supplemental insurance product to enroll in.\",\n      \"enum\": [\n        \"accident\",\n        \"critical_illness\",\n        \"cancer\",\n        \"hospital_indemnity\",\n        \"disability\",\n        \"life\"\n   \
  \   ],\n      \"example\": \"accident\"\n    },\n    \"coverage_level\": {\n      \"type\": \"string\",\n      \"description\": \"Coverage level for the enrollment.\",\n      \"enum\": [\n        \"employee_only\",\n        \"employee_spouse\",\n        \"employee_children\",\n        \"family\"\n      ],\n      \"example\": \"employee_only\"\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested effective date for coverage.\",\n      \"example\": \"2025-01-01\"\n    },\n    \"dependents\": {\n      \"type\": \"array\",\n      \"description\": \"List of dependents to include in family coverage.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Dependent\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"employee_id\",\n    \"group_id\",\n    \"product_type\",\n    \"coverage_level\",\n    \"effective_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-enrollment-request-schema.json
tags: []
title: EnrollmentRequest
---
