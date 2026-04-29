---
description: ''
layout: schema
name: Worker
properties_list:
- description: The Workday ID of the worker.
  name: id
  type: string
- description: A display descriptor for the worker.
  name: descriptor
  type: string
- description: The employee or contingent worker ID.
  name: workerID
  type: string
- description: ''
  name: primaryWorkEmail
  type: string
- description: ''
  name: primaryWorkPhone
  type: string
- description: ''
  name: businessTitle
  type: string
- description: The hire date for the worker.
  name: hireDate
  type: string
- description: The termination date, if applicable.
  name: terminationDate
  type: string
- description: Whether the worker is a manager.
  name: isManager
  type: boolean
- description: The external ID for the worker.
  name: externalID
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-worker-schema.json
slug: hcm-worker
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Worker\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the worker.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the worker.\"\n    },\n    \"workerID\": {\n      \"type\": \"string\",\n      \"description\": \"The employee or contingent worker ID.\"\n    },\n    \"primaryWorkEmail\": {\n      \"type\": \"string\"\n    },\n    \"primaryWorkPhone\": {\n      \"type\": \"string\"\n    },\n    \"businessTitle\": {\n      \"type\": \"string\"\n    },\n    \"hireDate\": {\n      \"type\": \"string\",\n      \"description\": \"The hire date for the worker.\"\n    },\n    \"terminationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The termination date, if applicable.\"\n    },\n    \"isManager\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the worker is a manager.\"\n    },\n    \"externalID\": {\n      \"type\": \"string\",\n      \"description\": \"The external ID for the worker.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-worker-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Worker
---
