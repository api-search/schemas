---
description: Contract from LinkedIn API
layout: schema
name: Contract
properties_list:
- description: The URN of this Sales Navigator contract
  name: contract
  type: string
- description: The name of this contract, appropriate for display to an end-user
  name: name
  type: string
- description: Additional information about the contract
  name: description
  type: string
- description: Indicates whether the user can export data for this contract
  name: hasReportingAccess
  type: boolean
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-contract-schema.json
slug: linkedin-sales-navigator-contract
source_filename: linkedin-sales-navigator-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-contract-schema.json\",\n  \"title\": \"Contract\",\n  \"description\": \"Contract from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contract\": {\n      \"type\": \"string\",\n      \"description\": \"The URN of this Sales Navigator contract\",\n      \"example\": \"urn:li:salesContract:12345\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of this contract, appropriate for display to an end-user\",\n      \"example\": \"Enterprise Sales Contract\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Additional information about the contract\",\n      \"example\": \"Annual enterprise subscription for sales team\"\n    },\n    \"hasReportingAccess\": {\n     \
  \ \"type\": \"boolean\",\n      \"description\": \"Indicates whether the user can export data for this contract\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"contract\",\n    \"name\",\n    \"hasReportingAccess\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-contract-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Contract
---
