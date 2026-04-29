---
description: A joint insured entity registered under a policy
layout: schema
name: JointInsured
properties_list:
- description: Unique identifier for the joint insured
  name: jointInsuredId
  type: string
- description: Parent policy identifier
  name: policyId
  type: string
- description: Legal name of the joint insured company
  name: companyName
  type: string
- description: Company registration number
  name: registrationNumber
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country
  type: string
- description: Current status of the joint insured
  name: status
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-policy-joint_insured-schema.json
slug: trade-policy-joint_insured
source_filename: trade-policy-joint_insured-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-policy-joint_insured-schema.json\",\n  \"title\": \"JointInsured\",\n  \"type\": \"object\",\n  \"description\": \"A joint insured entity registered under a policy\",\n  \"properties\": {\n    \"jointInsuredId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the joint insured\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent policy identifier\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of the joint insured company\"\n    },\n    \"registrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Company registration number\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Current status of the joint insured\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-policy-joint_insured-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: JointInsured
---
