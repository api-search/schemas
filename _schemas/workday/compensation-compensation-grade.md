---
description: ''
layout: schema
name: CompensationGrade
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: isInactive
  type: boolean
- description: ''
  name: minimumAmount
  type: number
- description: ''
  name: midpointAmount
  type: number
- description: ''
  name: maximumAmount
  type: number
provider_name: Workday
provider_slug: workday
schema_file: json-schema/compensation-compensation-grade-schema.json
slug: compensation-compensation-grade
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompensationGrade\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"isInactive\": {\n      \"type\": \"boolean\"\n    },\n    \"minimumAmount\": {\n      \"type\": \"number\"\n    },\n    \"midpointAmount\": {\n      \"type\": \"number\"\n    },\n    \"maximumAmount\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/compensation-compensation-grade-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: CompensationGrade
---
