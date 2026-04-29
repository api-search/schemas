---
description: Issue schema from 1Factory API
layout: schema
name: Issue
properties_list:
- description: ''
  name: ID
  type: object
- description: The reference number for the NCR, Complaint, or CAPA
  name: number
  type: number
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
  name: customer_name
  type: object
- description: 'Your Organization''s custom identifier for customer NCRs (ex. Customer PO #)'
  name: customer_ident
  type: string
- description: ''
  name: supplier_name
  type: object
- description: 'Your Organization''s custom identifier for supplier NCRs (ex. Supplier Lot #)'
  name: supplier_ident
  type: string
- description: Type of NCR
  name: type
  type: string
- description: 'Your Organization''s custom primary identifier for manufacturing inspection identifiers. (ex. Job #)'
  name: mfg_insp_ident_1
  type: string
- description: 'Your Organization''s custom secondary identifier for manufacturing inspection identifiers. (ex. PO #)'
  name: mfg_insp_ident_2
  type: string
- description: 'Your Organization''s custom primary identifier for receiving inspection identifiers. (ex. Job #)'
  name: rec_insp_ident_1
  type: string
- description: 'Your Organization''s custom secondary identifier for receiving inspection identifiers. (ex. PO #)'
  name: rec_insp_ident_2
  type: string
- description: The number of parts in the lot of the NCR
  name: lot_quantity
  type: number
- description: The number of parts in the lot that were inspected as part of the NCR
  name: inspection_quantity
  type: number
- description: The number of parts rejected as part of the NCR
  name: defective_quantity
  type: number
- description: Business impact of the NCR
  name: impact
  type: string
- description: Where the problem for the NCR was detected.
  name: detected_at
  type: string
- description: A simple description of the problem.
  name: problem_type
  type: string
- description: The root cause of the problem.
  name: root_cause
  type: string
- description: The department or group that caused the problem.
  name: caused_by
  type: string
- description: Problem summary of the NCR.
  name: problem_summary
  type: string
- description: Cost of the NCR
  name: total_cost
  type: number
- description: Status of the NCR
  name: status
  type: string
- description: Status of all tasks on NCR.
  name: task_status
  type: string
- description: Number of tasks for the NCR.
  name: task_count
  type: number
- description: ''
  name: owner
  type: object
- description: ''
  name: created_by_name
  type: object
- description: ''
  name: created_on
  type: object
- description: ''
  name: updated_on
  type: object
- description: ''
  name: closed_on
  type: object
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-issue-schema.json
slug: 1factory-issue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-issue-schema.json\",\n  \"title\": \"Issue\",\n  \"description\": \"Issue schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"$ref\": \"#/components/schemas/ID\"\n    },\n    \"number\": {\n      \"type\": \"number\",\n      \"example\": 1234,\n      \"description\": \"The reference number for the NCR, Complaint, or CAPA\"\n    },\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"part_description\": {\n      \"$ref\": \"#/components/schemas/part_description\"\n    },\n    \"customer_name\": {\n      \"$ref\": \"#/components/schemas/customer_name\"\n    },\n    \"customer_ident\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n     \
  \ \"maxLength\": 255,\n      \"description\": \"Your Organization's custom identifier for customer NCRs (ex. Customer PO #)\",\n      \"example\": \"PO-1234\"\n    },\n    \"supplier_name\": {\n      \"$ref\": \"#/components/schemas/supplier_name\"\n    },\n    \"supplier_ident\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Your Organization's custom identifier for supplier NCRs (ex. Supplier Lot #)\",\n      \"example\": \"123456\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Type of NCR\",\n      \"example\": \"Rcvg.\",\n      \"enum\": [\n        \"Rcvg.\",\n        \"Mfg.\",\n        \"Field\",\n        \"Cust.\",\n        \"Devn.\"\n      ]\n    },\n    \"mfg_insp_ident_1\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Your Organization's custom primary identifier for manufacturing inspection\
  \ identifiers. (ex. Job #)\",\n      \"example\": \"job-20240003\"\n    },\n    \"mfg_insp_ident_2\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Your Organization's custom secondary identifier for manufacturing inspection identifiers. (ex. PO #)\",\n      \"example\": \"po-20240065\"\n    },\n    \"rec_insp_ident_1\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Your Organization's custom primary identifier for receiving inspection identifiers. (ex. Job #)\",\n      \"example\": \"job-20240003\"\n    },\n    \"rec_insp_ident_2\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Your Organization's custom secondary identifier for receiving inspection identifiers. (ex. PO #)\",\n      \"example\": \"po-20240065\"\n    },\n    \"lot_quantity\": {\n      \"type\": \"number\",\n      \"nullable\":\
  \ false,\n      \"description\": \"The number of parts in the lot of the NCR\",\n      \"example\": 100\n    },\n    \"inspection_quantity\": {\n      \"type\": \"number\",\n      \"nullable\": false,\n      \"description\": \"The number of parts in the lot that were inspected as part of the NCR\",\n      \"example\": 10\n    },\n    \"defective_quantity\": {\n      \"type\": \"number\",\n      \"nullable\": false,\n      \"description\": \"The number of parts rejected as part of the NCR\",\n      \"example\": 3\n    },\n    \"impact\": {\n      \"type\": \"string\",\n      \"description\": \"Business impact of the NCR\",\n      \"example\": \"LOW\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\"\n      ]\n    },\n    \"detected_at\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Where the problem for the NCR was detected.\",\n      \"example\": \"Final Inspection\"\n    },\n    \"problem_type\": {\n      \"type\": \"string\"\
  ,\n      \"nullable\": true,\n      \"description\": \"A simple description of the problem.\",\n      \"example\": \"Out-of-spec\"\n    },\n    \"root_cause\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"The root cause of the problem.\",\n      \"example\": \"Machining Error\"\n    },\n    \"caused_by\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"The department or group that caused the problem.\",\n      \"example\": \"Engineering\"\n    },\n    \"problem_summary\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Problem summary of the NCR.\",\n      \"example\": \"Manufacturing defect\"\n    },\n    \"total_cost\": {\n      \"type\": \"number\",\n      \"nullable\": true,\n      \"description\": \"Cost of the NCR\",\n      \"example\": 1000.0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the NCR\"\
  ,\n      \"example\": \"OPEN\",\n      \"enum\": [\n        \"OPEN\",\n        \"CLOSED\"\n      ]\n    },\n    \"task_status\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"description\": \"Status of all tasks on NCR.\",\n      \"example\": \"OPEN\",\n      \"enum\": [\n        \"N/A\",\n        \"OPEN\",\n        \"CLOSED\"\n      ]\n    },\n    \"task_count\": {\n      \"type\": \"number\",\n      \"nullable\": false,\n      \"description\": \"Number of tasks for the NCR.\",\n      \"example\": 3\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/owner\"\n    },\n    \"created_by_name\": {\n      \"$ref\": \"#/components/schemas/created_by_username\"\n    },\n    \"created_on\": {\n      \"$ref\": \"#/components/schemas/created_on\"\n    },\n    \"updated_on\": {\n      \"$ref\": \"#/components/schemas/updated_on\"\n    },\n    \"closed_on\": {\n      \"$ref\": \"#/components/schemas/closed_on\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-issue-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Issue
---
