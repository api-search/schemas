---
description: CostEstimateAssumptions schema from Adyen API
layout: schema
name: CostEstimateAssumptions
properties_list:
- description: If true, the cardholder is expected to successfully authorise via 3D Secure.
  name: assume3DSecureAuthenticated
  type: boolean
- description: If true, the transaction is expected to have valid Level 3 data.
  name: assumeLevel3Data
  type: boolean
- description: If not zero, the number of installments.
  name: installments
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-cost-estimate-assumptions-schema.json
slug: binlookup-cost-estimate-assumptions
source_filename: binlookup-cost-estimate-assumptions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-cost-estimate-assumptions-schema.json\",\n  \"title\": \"CostEstimateAssumptions\",\n  \"description\": \"CostEstimateAssumptions schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assume3DSecureAuthenticated\": {\n      \"description\": \"If true, the cardholder is expected to successfully authorise via 3D Secure.\",\n      \"type\": \"boolean\"\n    },\n    \"assumeLevel3Data\": {\n      \"description\": \"If true, the transaction is expected to have valid Level 3 data.\",\n      \"type\": \"boolean\"\n    },\n    \"installments\": {\n      \"description\": \"If not zero, the number of installments.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-cost-estimate-assumptions-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CostEstimateAssumptions
---
