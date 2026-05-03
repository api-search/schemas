---
description: A company (customer organization) record in Schematic, representing a billable entity with features, plans, and entitlements.
layout: schema
name: Schematic Company
properties_list:
- description: Unique Schematic company identifier.
  name: id
  type: string
- description: Display name of the company.
  name: name
  type: string
- description: External system keys used to identify the company (e.g., Stripe customer ID, Salesforce account ID).
  name: keys
  type: object
- description: Custom metadata attributes for the company.
  name: traits
  type: object
- description: The active subscription plan for the company.
  name: plan
  type: object
- description: Trait values associated with this company.
  name: entityTraits
  type: array
- description: ISO 8601 timestamp when the company was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the company was last updated.
  name: updatedAt
  type: string
- description: ISO 8601 timestamp of the most recent activity for this company.
  name: lastSeenAt
  type: string
- description: Number of users associated with this company.
  name: userCount
  type: integer
provider_name: Schematic
provider_slug: schematic
schema_file: json-schema/schematic-company-schema.json
slug: schematic-company
source_filename: schematic-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.schematichq.com/schemas/company\",\n  \"title\": \"Schematic Company\",\n  \"description\": \"A company (customer organization) record in Schematic, representing a billable entity with features, plans, and entitlements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Schematic company identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the company.\"\n    },\n    \"keys\": {\n      \"type\": \"object\",\n      \"description\": \"External system keys used to identify the company (e.g., Stripe customer ID, Salesforce account ID).\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"traits\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata attributes for the company.\",\n      \"additionalProperties\": true\n\
  \    },\n    \"plan\": {\n      \"$ref\": \"#/$defs/PlanRef\",\n      \"description\": \"The active subscription plan for the company.\"\n    },\n    \"entityTraits\": {\n      \"type\": \"array\",\n      \"description\": \"Trait values associated with this company.\",\n      \"items\": { \"$ref\": \"#/$defs/EntityTrait\" }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the company was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the company was last updated.\"\n    },\n    \"lastSeenAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the most recent activity for this company.\"\n    },\n    \"userCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users associated with this company.\"\n    }\n\
  \  },\n  \"required\": [\"id\", \"name\"],\n  \"$defs\": {\n    \"PlanRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"EntityTrait\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"traitDefinitionId\": { \"type\": \"string\" },\n        \"value\": {}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/json-schema/schematic-company-schema.json
tags:
- Billing
- Entitlements
- Feature Flags
- Feature Management
- FinOps
- Metering
- Pricing
- SaaS
title: Schematic Company
---
