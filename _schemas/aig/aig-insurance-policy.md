---
description: An AIG insurance policy covering insured risks
layout: schema
name: InsurancePolicy
properties_list:
- description: Unique policy identifier
  name: policy_number
  type: string
- description: Type of insurance policy
  name: policy_type
  type: string
- description: Name of the insured entity
  name: insured_name
  type: string
- description: Policy effective date
  name: effective_date
  type: string
- description: Policy expiration date
  name: expiration_date
  type: string
- description: Annual premium amount in USD
  name: premium
  type: number
- description: Policy coverage limit in USD
  name: coverage_limit
  type: number
- description: Policy deductible amount in USD
  name: deductible
  type: number
- description: Policy status
  name: status
  type: string
provider_name: AIG
provider_slug: aig
schema_file: json-schema/aig-insurance-policy-schema.json
slug: aig-insurance-policy
source_filename: aig-insurance-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-insurance-policy-schema.json\",\n  \"title\": \"InsurancePolicy\",\n  \"description\": \"An AIG insurance policy covering insured risks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_number\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy identifier\",\n      \"example\": \"AIG-GL-2024-001234\"\n    },\n    \"policy_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of insurance policy\",\n      \"example\": \"Commercial General Liability\"\n    },\n    \"insured_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the insured entity\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"effective_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy effective date\",\n      \"example\"\
  : \"2024-01-01\"\n    },\n    \"expiration_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy expiration date\",\n      \"example\": \"2025-01-01\"\n    },\n    \"premium\": {\n      \"type\": \"number\",\n      \"description\": \"Annual premium amount in USD\",\n      \"example\": 125000.0\n    },\n    \"coverage_limit\": {\n      \"type\": \"number\",\n      \"description\": \"Policy coverage limit in USD\",\n      \"example\": 5000000.0\n    },\n    \"deductible\": {\n      \"type\": \"number\",\n      \"description\": \"Policy deductible amount in USD\",\n      \"example\": 50000.0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Policy status\",\n      \"example\": \"Active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-insurance-policy-schema.json
tags:
- Insurance
- Financial Services
- Property Casualty
- Cyber Insurance
- Enterprise
title: InsurancePolicy
---
