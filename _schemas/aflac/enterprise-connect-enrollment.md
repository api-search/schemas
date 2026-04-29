---
description: A supplemental insurance enrollment record for an employee.
layout: schema
name: Enrollment
properties_list:
- description: Unique enrollment identifier.
  name: enrollment_id
  type: string
- description: Employee identifier.
  name: employee_id
  type: string
- description: Employer group identifier.
  name: group_id
  type: string
- description: Associated policy identifier assigned upon enrollment.
  name: policy_id
  type: string
- description: Type of supplemental insurance product.
  name: product_type
  type: string
- description: Coverage level selected by the employee.
  name: coverage_level
  type: string
- description: Current enrollment status.
  name: status
  type: string
- description: Date the coverage became effective.
  name: effective_date
  type: string
- description: Date the coverage was terminated, if applicable.
  name: termination_date
  type: string
- description: Monthly premium amount in USD.
  name: monthly_premium
  type: number
- description: Timestamp when the enrollment was created.
  name: created_at
  type: string
- description: Timestamp when the enrollment was last updated.
  name: updated_at
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-enrollment-schema.json
slug: enterprise-connect-enrollment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-enrollment-schema.json\",\n  \"title\": \"Enrollment\",\n  \"description\": \"A supplemental insurance enrollment record for an employee.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrollment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique enrollment identifier.\",\n      \"example\": \"ENR-500123\"\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee identifier.\",\n      \"example\": \"EMP-789012\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employer group identifier.\",\n      \"example\": \"GRP-123456\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated policy identifier assigned upon enrollment.\",\n      \"example\": \"POL-987654\"\
  \n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of supplemental insurance product.\",\n      \"enum\": [\n        \"accident\",\n        \"critical_illness\",\n        \"cancer\",\n        \"hospital_indemnity\",\n        \"disability\",\n        \"life\"\n      ],\n      \"example\": \"accident\"\n    },\n    \"coverage_level\": {\n      \"type\": \"string\",\n      \"description\": \"Coverage level selected by the employee.\",\n      \"enum\": [\n        \"employee_only\",\n        \"employee_spouse\",\n        \"employee_children\",\n        \"family\"\n      ],\n      \"example\": \"family\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current enrollment status.\",\n      \"enum\": [\n        \"active\",\n        \"pending\",\n        \"terminated\"\n      ],\n      \"example\": \"active\"\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\"\
  : \"Date the coverage became effective.\",\n      \"example\": \"2025-01-01\"\n    },\n    \"termination_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the coverage was terminated, if applicable.\",\n      \"example\": \"2025-12-31\"\n    },\n    \"monthly_premium\": {\n      \"type\": \"number\",\n      \"description\": \"Monthly premium amount in USD.\",\n      \"example\": 18.5\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the enrollment was created.\",\n      \"example\": \"2024-11-01T10:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the enrollment was last updated.\",\n      \"example\": \"2025-01-01T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-enrollment-schema.json
tags: []
title: Enrollment
---
