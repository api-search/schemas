---
description: An insurance claim filed under an AIG policy
layout: schema
name: InsuranceClaim
properties_list:
- description: Unique claim identifier
  name: claim_number
  type: string
- description: Associated policy number
  name: policy_number
  type: string
- description: Date of loss occurrence
  name: loss_date
  type: string
- description: Date claim was reported
  name: reported_date
  type: string
- description: Description of the loss or damage
  name: loss_description
  type: string
- description: Estimated loss amount in USD
  name: loss_amount
  type: number
- description: Current claim status
  name: claim_status
  type: string
- description: Name of assigned claims adjuster
  name: adjuster_name
  type: string
provider_name: AIG
provider_slug: aig
schema_file: json-schema/aig-insurance-claim-schema.json
slug: aig-insurance-claim
source_filename: aig-insurance-claim-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-insurance-claim-schema.json\",\n  \"title\": \"InsuranceClaim\",\n  \"description\": \"An insurance claim filed under an AIG policy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"claim_number\": {\n      \"type\": \"string\",\n      \"description\": \"Unique claim identifier\",\n      \"example\": \"CLM-2024-567890\"\n    },\n    \"policy_number\": {\n      \"type\": \"string\",\n      \"description\": \"Associated policy number\",\n      \"example\": \"AIG-GL-2024-001234\"\n    },\n    \"loss_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of loss occurrence\",\n      \"example\": \"2024-06-15\"\n    },\n    \"reported_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date claim was reported\",\n      \"example\"\
  : \"2024-06-17\"\n    },\n    \"loss_description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the loss or damage\",\n      \"example\": \"Property damage due to fire in warehouse facility\"\n    },\n    \"loss_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated loss amount in USD\",\n      \"example\": 250000.0\n    },\n    \"claim_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current claim status\",\n      \"example\": \"Under Investigation\"\n    },\n    \"adjuster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of assigned claims adjuster\",\n      \"example\": \"Jane Smith\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-insurance-claim-schema.json
tags:
- Insurance
- Financial Services
- Property Casualty
- Cyber Insurance
- Enterprise
title: InsuranceClaim
---
