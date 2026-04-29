---
description: ''
layout: schema
name: ScorecardResult
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: currentBasePayAmount
  type: number
- description: ''
  name: proposedBasePayAmount
  type: number
- description: ''
  name: percentChange
  type: number
- description: ''
  name: meritAmount
  type: number
- description: ''
  name: promotionAmount
  type: number
provider_name: Workday
provider_slug: workday
schema_file: json-schema/compensation-scorecard-result-schema.json
slug: compensation-scorecard-result
source_filename: compensation-scorecard-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScorecardResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"currentBasePayAmount\": {\n      \"type\": \"number\"\n    },\n    \"proposedBasePayAmount\": {\n      \"type\": \"number\"\n    },\n    \"percentChange\": {\n      \"type\": \"number\"\n    },\n    \"meritAmount\": {\n      \"type\": \"number\"\n    },\n    \"promotionAmount\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/compensation-scorecard-result-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ScorecardResult
---
