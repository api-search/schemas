---
description: Request body for adding a joint insured to a policy
layout: schema
name: AddJointInsuredRequest
properties_list:
- description: Legal name of the company to add as joint insured
  name: companyName
  type: string
- description: Company registration number
  name: registrationNumber
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-policy-add_joint_insured_request-schema.json
slug: trade-policy-add_joint_insured_request
source_filename: trade-policy-add_joint_insured_request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-policy-add_joint_insured_request-schema.json\",\n  \"title\": \"AddJointInsuredRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for adding a joint insured to a policy\",\n  \"properties\": {\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of the company to add as joint insured\"\n    },\n    \"registrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Company registration number\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    }\n  },\n  \"required\": [\n    \"companyName\",\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-policy-add_joint_insured_request-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: AddJointInsuredRequest
---
