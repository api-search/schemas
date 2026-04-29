---
description: ''
layout: schema
name: JobRequisition
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: requisitionNumber
  type: string
- description: ''
  name: jobTitle
  type: string
- description: The status of the requisition (e.g., Open, Filled, Closed).
  name: status
  type: string
- description: ''
  name: numberOfOpenings
  type: integer
- description: ''
  name: createdOn
  type: string
- description: ''
  name: targetHireDate
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/recruiting-job-requisition-schema.json
slug: recruiting-job-requisition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobRequisition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"requisitionNumber\": {\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the requisition (e.g., Open, Filled, Closed).\"\n    },\n    \"numberOfOpenings\": {\n      \"type\": \"integer\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\"\n    },\n    \"targetHireDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/recruiting-job-requisition-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: JobRequisition
---
