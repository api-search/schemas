---
description: ADP Worker (employee or contractor)
layout: schema
name: Worker
properties_list:
- description: ADP Associate Object Identifier - unique worker identifier
  name: associateOID
  type: string
- description: ''
  name: workerID
  type: object
- description: ''
  name: workerDates
  type: object
- description: ''
  name: workAssignments
  type: array
- description: ''
  name: customFieldGroup
  type: object
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-workers-worker-schema.json
slug: adp-workers-worker
source_filename: adp-workers-worker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Worker\",\n  \"type\": \"object\",\n  \"description\": \"ADP Worker (employee or contractor)\",\n  \"properties\": {\n    \"associateOID\": {\n      \"type\": \"string\",\n      \"description\": \"ADP Associate Object Identifier - unique worker identifier\"\n    },\n    \"workerID\": {\n      \"type\": \"object\"\n    },\n    \"workerDates\": {\n      \"type\": \"object\"\n    },\n    \"workAssignments\": {\n      \"type\": \"array\"\n    },\n    \"customFieldGroup\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-workers-worker-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: Worker
---
