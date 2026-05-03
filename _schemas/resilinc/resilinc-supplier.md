---
description: JSON Schema for a Resilinc supplier record in the supply chain risk management platform. Represents a supplier organization tracked for risk monitoring and disruption analysis.
layout: schema
name: Resilinc Supplier
properties_list:
- description: Unique supplier identifier.
  name: id
  type: string
- description: Supplier organization name.
  name: name
  type: string
- description: Country where the supplier is located.
  name: country
  type: string
- description: Geographic region.
  name: region
  type: string
- description: City where the supplier operates.
  name: city
  type: string
- description: Industry sector of the supplier.
  name: industry
  type: string
- description: Supply chain tier level (1 = direct supplier, 2+ = sub-tier).
  name: tier
  type: integer
- description: Composite risk score (0-100, higher = more risk).
  name: risk_score
  type: number
- description: Current supplier status.
  name: status
  type: string
- description: Parts or components sourced from this supplier.
  name: parts
  type: array
- description: Manufacturing or operational sites.
  name: sites
  type: array
- description: Record creation timestamp.
  name: created_at
  type: string
- description: Record last updated timestamp.
  name: updated_at
  type: string
provider_name: Resilinc
provider_slug: resilinc
schema_file: json-schema/resilinc-supplier-schema.json
slug: resilinc-supplier
source_filename: resilinc-supplier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resilinc/json-schema/resilinc-supplier-schema.json\",\n  \"title\": \"Resilinc Supplier\",\n  \"description\": \"JSON Schema for a Resilinc supplier record in the supply chain risk management platform. Represents a supplier organization tracked for risk monitoring and disruption analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique supplier identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier organization name.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country where the supplier is located.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic region.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the supplier\
  \ operates.\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry sector of the supplier.\"\n    },\n    \"tier\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Supply chain tier level (1 = direct supplier, 2+ = sub-tier).\"\n    },\n    \"risk_score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Composite risk score (0-100, higher = more risk).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"under_review\", \"critical\"],\n      \"description\": \"Current supplier status.\"\n    },\n    \"parts\": {\n      \"type\": \"array\",\n      \"description\": \"Parts or components sourced from this supplier.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"part_number\": { \"type\": \"string\" },\n          \"description\"\
  : { \"type\": \"string\" }\n        }\n      }\n    },\n    \"sites\": {\n      \"type\": \"array\",\n      \"description\": \"Manufacturing or operational sites.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" },\n          \"address\": { \"type\": \"string\" },\n          \"country\": { \"type\": \"string\" },\n          \"lat\": { \"type\": \"number\" },\n          \"lon\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last updated timestamp.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"country\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resilinc/refs/heads/main/json-schema/resilinc-supplier-schema.json
tags:
- Supply Chain
- Risk Management
- Supplier Intelligence
- Disruption Monitoring
- AI
title: Resilinc Supplier
---
