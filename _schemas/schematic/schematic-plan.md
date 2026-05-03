---
description: A subscription plan in Schematic that bundles features and entitlements for customer billing.
layout: schema
name: Schematic Plan
properties_list:
- description: Unique Schematic plan identifier.
  name: id
  type: string
- description: Display name of the plan.
  name: name
  type: string
- description: Human-readable description of the plan.
  name: description
  type: string
- description: Whether this is a base subscription plan or an add-on.
  name: planType
  type: string
- description: Whether this plan version is the current published version.
  name: current
  type: boolean
- description: Feature entitlements included in this plan.
  name: entitlements
  type: array
- description: The associated billing product in Stripe or billing provider.
  name: billingProduct
  type: object
- description: ''
  name: monthlyPrice
  type: object
- description: ''
  name: yearlyPrice
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Schematic
provider_slug: schematic
schema_file: json-schema/schematic-plan-schema.json
slug: schematic-plan
source_filename: schematic-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.schematichq.com/schemas/plan\",\n  \"title\": \"Schematic Plan\",\n  \"description\": \"A subscription plan in Schematic that bundles features and entitlements for customer billing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Schematic plan identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the plan.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the plan.\"\n    },\n    \"planType\": {\n      \"type\": \"string\",\n      \"enum\": [\"base\", \"add_on\"],\n      \"description\": \"Whether this is a base subscription plan or an add-on.\"\n    },\n    \"current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this plan version is the current published version.\"\
  \n    },\n    \"entitlements\": {\n      \"type\": \"array\",\n      \"description\": \"Feature entitlements included in this plan.\",\n      \"items\": { \"$ref\": \"#/$defs/Entitlement\" }\n    },\n    \"billingProduct\": {\n      \"$ref\": \"#/$defs/BillingProductRef\",\n      \"description\": \"The associated billing product in Stripe or billing provider.\"\n    },\n    \"monthlyPrice\": {\n      \"$ref\": \"#/$defs/BillingPriceRef\"\n    },\n    \"yearlyPrice\": {\n      \"$ref\": \"#/$defs/BillingPriceRef\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"planType\"],\n  \"$defs\": {\n    \"Entitlement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"feature\": {\n          \"type\": \"object\",\n          \"properties\": {\n        \
  \    \"id\": { \"type\": \"string\" },\n            \"name\": { \"type\": \"string\" }\n          }\n        },\n        \"valueType\": {\n          \"type\": \"string\",\n          \"enum\": [\"boolean\", \"numeric\", \"unlimited\", \"trait\"]\n        },\n        \"numericValue\": {\n          \"type\": \"integer\",\n          \"nullable\": true\n        }\n      }\n    },\n    \"BillingProductRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"externalId\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"BillingPriceRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"externalId\": { \"type\": \"string\" },\n        \"price\": { \"type\": \"integer\" },\n        \"currency\": { \"type\": \"string\" },\n        \"interval\": { \"type\": \"string\", \"enum\": [\"month\", \"year\"] }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/json-schema/schematic-plan-schema.json
tags:
- Billing
- Entitlements
- Feature Flags
- Feature Management
- FinOps
- Metering
- Pricing
- SaaS
title: Schematic Plan
---
