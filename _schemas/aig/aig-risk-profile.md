---
description: Risk profile for an insured entity
layout: schema
name: RiskProfile
properties_list:
- description: Name of the insured entity
  name: entity_name
  type: string
- description: Industry classification
  name: industry
  type: string
- description: NAICS industry code
  name: naics_code
  type: string
- description: Annual revenue in USD
  name: annual_revenue
  type: number
- description: Number of employees
  name: employee_count
  type: integer
- description: List of business locations
  name: locations
  type: array
- description: Historical loss records
  name: loss_history
  type: array
provider_name: AIG
provider_slug: aig
schema_file: json-schema/aig-risk-profile-schema.json
slug: aig-risk-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-risk-profile-schema.json\",\n  \"title\": \"RiskProfile\",\n  \"description\": \"Risk profile for an insured entity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entity_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the insured entity\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification\",\n      \"example\": \"Manufacturing\"\n    },\n    \"naics_code\": {\n      \"type\": \"string\",\n      \"description\": \"NAICS industry code\",\n      \"example\": \"332999\"\n    },\n    \"annual_revenue\": {\n      \"type\": \"number\",\n      \"description\": \"Annual revenue in USD\",\n      \"example\": 50000000.0\n    },\n    \"employee_count\": {\n      \"type\": \"integer\",\n    \
  \  \"description\": \"Number of employees\",\n      \"example\": 500\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"description\": \"List of business locations\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"loss_history\": {\n      \"type\": \"array\",\n      \"description\": \"Historical loss records\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-risk-profile-schema.json
tags:
- Insurance
- Financial Services
- Property Casualty
- Cyber Insurance
- Enterprise
title: RiskProfile
---
