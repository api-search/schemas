---
description: Schema for an institution returned by the HMDA Institutions API.
layout: schema
name: CFPB HMDA Institution
properties_list:
- description: ''
  name: lei
  type: string
- description: ''
  name: activityYear
  type: integer
- description: ''
  name: agency
  type: integer
- description: ''
  name: institutionType
  type: string
- description: ''
  name: institutionId2017
  type: string
- description: ''
  name: taxId
  type: string
- description: ''
  name: rssd
  type: integer
- description: ''
  name: respondent
  type: object
- description: ''
  name: parent
  type: object
- description: ''
  name: assets
  type: integer
- description: ''
  name: otherLenderCode
  type: integer
- description: ''
  name: topHolder
  type: object
- description: ''
  name: hmdaFiler
  type: boolean
- description: ''
  name: quarterlyFiler
  type: boolean
- description: ''
  name: quarterlyFilerHasFiledQ1
  type: boolean
- description: ''
  name: quarterlyFilerHasFiledQ2
  type: boolean
- description: ''
  name: quarterlyFilerHasFiledQ3
  type: boolean
provider_name: Consumer Financial Protection Bureau
provider_slug: consumer-financial-protection-bureau
schema_file: json-schema/cfpb-hmda-institution-schema.json
slug: cfpb-hmda-institution
source_filename: cfpb-hmda-institution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/json-schema/cfpb-hmda-institution-schema.json\",\n  \"title\": \"CFPB HMDA Institution\",\n  \"description\": \"Schema for an institution returned by the HMDA Institutions API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lei\": { \"type\": \"string\", \"minLength\": 20, \"maxLength\": 20 },\n    \"activityYear\": { \"type\": \"integer\" },\n    \"agency\": { \"type\": \"integer\" },\n    \"institutionType\": { \"type\": \"string\" },\n    \"institutionId2017\": { \"type\": \"string\" },\n    \"taxId\": { \"type\": \"string\" },\n    \"rssd\": { \"type\": \"integer\" },\n    \"respondent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\", \"minLength\": 2, \"maxLength\": 2 },\n        \"city\"\
  : { \"type\": \"string\" }\n      }\n    },\n    \"parent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"idRssd\": { \"type\": \"integer\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"assets\": { \"type\": \"integer\" },\n    \"otherLenderCode\": { \"type\": \"integer\" },\n    \"topHolder\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"idRssd\": { \"type\": \"integer\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"hmdaFiler\": { \"type\": \"boolean\" },\n    \"quarterlyFiler\": { \"type\": \"boolean\" },\n    \"quarterlyFilerHasFiledQ1\": { \"type\": \"boolean\" },\n    \"quarterlyFilerHasFiledQ2\": { \"type\": \"boolean\" },\n    \"quarterlyFilerHasFiledQ3\": { \"type\": \"boolean\" }\n  },\n  \"required\": [\"lei\", \"activityYear\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/json-schema/cfpb-hmda-institution-schema.json
tags:
- Banking
- Complaints
- Consumer Protection
- Federal Government
- Financial Services
- HMDA
- Mortgages
- Open Data
title: CFPB HMDA Institution
---
