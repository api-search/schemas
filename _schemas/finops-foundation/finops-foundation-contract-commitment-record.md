---
description: A contract commitment record as defined in FOCUS v1.3. Isolates contract terms including start and end dates, remaining units, and descriptions from cost and usage rows.
layout: schema
name: FOCUS Contract Commitment Record
properties_list:
- description: The unique identifier assigned to a commitment discount by the provider.
  name: CommitmentDiscountId
  type: string
- description: The display name assigned to a commitment discount.
  name: CommitmentDiscountName
  type:
  - string
  - 'null'
- description: A provider-assigned label describing the type of commitment discount.
  name: CommitmentDiscountType
  type:
  - string
  - 'null'
- description: Whether the commitment discount is based on usage quantity or cost.
  name: CommitmentDiscountCategory
  type: string
- description: The start date and time of the contract commitment.
  name: CommitmentStartDate
  type: string
- description: The end date and time of the contract commitment.
  name: CommitmentEndDate
  type: string
- description: The total quantity of the commitment purchased.
  name: CommitmentTotalQuantity
  type:
  - number
  - 'null'
- description: The remaining quantity of the commitment that has not yet been consumed.
  name: CommitmentRemainingQuantity
  type:
  - number
  - 'null'
- description: The unit of measurement for the commitment quantity.
  name: CommitmentUnit
  type:
  - string
  - 'null'
- description: A human-readable description of the contract commitment.
  name: CommitmentDescription
  type:
  - string
  - 'null'
- description: The unique identifier for the billing account associated with the commitment.
  name: BillingAccountId
  type: string
- description: The display name for the billing account.
  name: BillingAccountName
  type:
  - string
  - 'null'
- description: The name of the entity that made the commitment discount available.
  name: ProviderName
  type: string
provider_name: FinOps Foundation
provider_slug: finops-foundation
schema_file: json-schema/finops-foundation-contract-commitment-record-schema.json
slug: finops-foundation-contract-commitment-record
source_filename: finops-foundation-contract-commitment-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/json-schema/finops-foundation-contract-commitment-record-schema.json\",\n  \"title\": \"FOCUS Contract Commitment Record\",\n  \"description\": \"A contract commitment record as defined in FOCUS v1.3. Isolates contract terms including start and end dates, remaining units, and descriptions from cost and usage rows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CommitmentDiscountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to a commitment discount by the provider.\"\n    },\n    \"CommitmentDiscountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name assigned to a commitment discount.\"\n    },\n    \"CommitmentDiscountType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A provider-assigned label\
  \ describing the type of commitment discount.\"\n    },\n    \"CommitmentDiscountCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\"Spend\", \"Usage\"],\n      \"description\": \"Whether the commitment discount is based on usage quantity or cost.\"\n    },\n    \"CommitmentStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start date and time of the contract commitment.\"\n    },\n    \"CommitmentEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end date and time of the contract commitment.\"\n    },\n    \"CommitmentTotalQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The total quantity of the commitment purchased.\"\n    },\n    \"CommitmentRemainingQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The remaining quantity of the commitment that has not yet been consumed.\"\n    },\n    \"CommitmentUnit\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unit of measurement for the commitment quantity.\"\n    },\n    \"CommitmentDescription\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A human-readable description of the contract commitment.\"\n    },\n    \"BillingAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the billing account associated with the commitment.\"\n    },\n    \"BillingAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name for the billing account.\"\n    },\n    \"ProviderName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity that made the commitment discount available.\"\n    }\n  },\n  \"required\": [\n    \"CommitmentDiscountId\",\n    \"CommitmentDiscountCategory\",\n    \"CommitmentStartDate\",\n    \"CommitmentEndDate\",\n    \"BillingAccountId\",\n    \"ProviderName\"\n  ],\n  \"additionalProperties\"\
  : true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/json-schema/finops-foundation-contract-commitment-record-schema.json
tags:
- Budgets
- Costs
- FinOps
title: FOCUS Contract Commitment Record
---
