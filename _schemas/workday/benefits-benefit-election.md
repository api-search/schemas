---
description: ''
layout: schema
name: BenefitElection
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The status of the election (e.g., Elected, Waived).
  name: electionStatus
  type: string
- description: ''
  name: coverageBeginDate
  type: string
- description: ''
  name: coverageEndDate
  type: string
- description: ''
  name: employeeCost
  type: number
- description: ''
  name: employerCost
  type: number
- description: ''
  name: dependents
  type: array
- description: ''
  name: beneficiaries
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/benefits-benefit-election-schema.json
slug: benefits-benefit-election
source_filename: benefits-benefit-election-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BenefitElection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"electionStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the election (e.g., Elected, Waived).\"\n    },\n    \"coverageBeginDate\": {\n      \"type\": \"string\"\n    },\n    \"coverageEndDate\": {\n      \"type\": \"string\"\n    },\n    \"employeeCost\": {\n      \"type\": \"number\"\n    },\n    \"employerCost\": {\n      \"type\": \"number\"\n    },\n    \"dependents\": {\n      \"type\": \"array\"\n    },\n    \"beneficiaries\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/benefits-benefit-election-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: BenefitElection
---
