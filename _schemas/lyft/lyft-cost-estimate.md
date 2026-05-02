---
description: An estimated cost, distance, and duration for a Lyft ride between two locations for a specific ride type.
layout: schema
name: Lyft Cost Estimate
properties_list:
- description: Identifier for the type of Lyft ride.
  name: ride_type
  type: string
- description: Human-readable name for the ride type.
  name: display_name
  type: string
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Lower bound of the estimated cost in cents.
  name: estimated_cost_cents_min
  type: integer
- description: Upper bound of the estimated cost in cents.
  name: estimated_cost_cents_max
  type: integer
- description: Estimated distance of the ride in miles.
  name: estimated_distance_miles
  type: number
- description: Estimated duration of the ride in seconds.
  name: estimated_duration_seconds
  type: integer
- description: Current Prime Time percentage applied to the cost estimate, formatted as a percentage string such as 25%.
  name: primetime_percentage
  type: string
- description: A token that must be included when requesting a ride during Prime Time pricing.
  name: primetime_confirmation_token
  type: string
provider_name: lyft
provider_slug: lyft
schema_file: json-schema/lyft-cost-estimate-schema.json
slug: lyft-cost-estimate
source_filename: lyft-cost-estimate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://lyft.com/schemas/lyft/cost-estimate.json\",\n  \"title\": \"Lyft Cost Estimate\",\n  \"description\": \"An estimated cost, distance, and duration for a Lyft ride between two locations for a specific ride type.\",\n  \"type\": \"object\",\n  \"required\": [\"ride_type\", \"estimated_cost_cents_min\", \"estimated_cost_cents_max\"],\n  \"properties\": {\n    \"ride_type\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the type of Lyft ride.\",\n      \"enum\": [\"lyft\", \"lyft_line\", \"lyft_plus\", \"lyft_premier\", \"lyft_lux\", \"lyft_luxsuv\"]\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the ride type.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"estimated_cost_cents_min\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Lower bound of the estimated cost in cents.\",\n      \"minimum\": 0\n    },\n    \"estimated_cost_cents_max\": {\n      \"type\": \"integer\",\n      \"description\": \"Upper bound of the estimated cost in cents.\",\n      \"minimum\": 0\n    },\n    \"estimated_distance_miles\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated distance of the ride in miles.\",\n      \"minimum\": 0\n    },\n    \"estimated_duration_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated duration of the ride in seconds.\",\n      \"minimum\": 0\n    },\n    \"primetime_percentage\": {\n      \"type\": \"string\",\n      \"description\": \"Current Prime Time percentage applied to the cost estimate, formatted as a percentage string such as 25%.\"\n    },\n    \"primetime_confirmation_token\": {\n      \"type\": \"string\",\n      \"description\": \"A token that must be included when requesting a ride during\
  \ Prime Time pricing.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/json-schema/lyft-cost-estimate-schema.json
tags: []
title: Lyft Cost Estimate
---
