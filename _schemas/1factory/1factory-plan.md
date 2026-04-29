---
description: Plan schema from 1Factory API
layout: schema
name: Plan
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: ''
  name: part_description
  type: object
- description: ''
  name: operation
  type: object
- description: ''
  name: project_identifier
  type: object
- description: ''
  name: status
  type: object
- description: Version of the plan.
  name: version
  type: number
- description: ''
  name: version_status
  type: string
- description: The status of a plan that requires approval before releasing or closing. (Availability depends on Organization settings.)
  name: approval_status
  type: string
- description: ''
  name: customer_name
  type: object
- description: ''
  name: supplier_name
  type: object
- description: ''
  name: supplier_number
  type: object
- description: If the plan is for a tabulated part.
  name: is_tabulated
  type: boolean
- description: If the plan is a spec library
  name: is_spec_lib
  type: boolean
- description: ''
  name: created_by_name
  type: object
- description: ''
  name: created_on
  type: object
- description: ''
  name: updated_on
  type: object
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-plan-schema.json
slug: 1factory-plan
source_filename: 1factory-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-plan-schema.json\",\n  \"title\": \"Plan\",\n  \"description\": \"Plan schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"$ref\": \"#/components/schemas/ID\"\n    },\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"part_description\": {\n      \"$ref\": \"#/components/schemas/part_description\"\n    },\n    \"operation\": {\n      \"$ref\": \"#/components/schemas/operation\"\n    },\n    \"project_identifier\": {\n      \"$ref\": \"#/components/schemas/project_identifier\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/status\"\n    },\n    \"version\": {\n      \"type\": \"number\",\n      \"description\": \"Version of the\
  \ plan.\",\n      \"example\": 4\n    },\n    \"version_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Draft\",\n        \"Approval\",\n        \"Released\",\n        \"Inactive\"\n      ]\n    },\n    \"approval_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"N/a\",\n        \"Pending\",\n        \"Assigned\",\n        \"Approved\",\n        \"Rejected\"\n      ],\n      \"description\": \"The status of a plan that requires approval before releasing or closing.\\n\\n(Availability depends on Organization settings.)\"\n    },\n    \"customer_name\": {\n      \"$ref\": \"#/components/schemas/customer_name\"\n    },\n    \"supplier_name\": {\n      \"$ref\": \"#/components/schemas/supplier_name\"\n    },\n    \"supplier_number\": {\n      \"$ref\": \"#/components/schemas/supplier_number\"\n    },\n    \"is_tabulated\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"If the plan is for\
  \ a tabulated part.\"\n    },\n    \"is_spec_lib\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"If the plan is a spec library\"\n    },\n    \"created_by_name\": {\n      \"$ref\": \"#/components/schemas/created_by_username\"\n    },\n    \"created_on\": {\n      \"$ref\": \"#/components/schemas/created_on\"\n    },\n    \"updated_on\": {\n      \"$ref\": \"#/components/schemas/updated_on\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-plan-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Plan
---
