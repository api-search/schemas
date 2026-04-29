---
description: Assignment of a pricing plan to a customer
layout: schema
name: PricingPlanAssignment
properties_list:
- description: Customer identifier
  name: customerId
  type: string
- description: Product or pricing plan identifier
  name: productId
  type: string
- description: Plan start time in Unix milliseconds
  name: startTime
  type: integer
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/billing-pricing-plan-assignment-schema.json
slug: billing-pricing-plan-assignment
source_filename: billing-pricing-plan-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-pricing-plan-assignment-schema.json\",\n  \"title\": \"PricingPlanAssignment\",\n  \"description\": \"Assignment of a pricing plan to a customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier\",\n      \"example\": \"customer-123456\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product or pricing plan identifier\",\n      \"example\": \"plan-standard\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Plan start time in Unix milliseconds\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-pricing-plan-assignment-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: PricingPlanAssignment
---
