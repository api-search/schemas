---
description: A Lyft ride type representing an available category of ride at a given location, including pricing details and passenger capacity.
layout: schema
name: Lyft Ride Type
properties_list:
- description: Identifier for the ride type.
  name: ride_type
  type: string
- description: Human-readable name for the ride type.
  name: display_name
  type: string
- description: Maximum number of passenger seats available for this ride type.
  name: seats
  type: integer
- description: URL to an image representing the ride type.
  name: image_url
  type: string
- description: Pricing breakdown for this ride type.
  name: pricing_details
  type: object
provider_name: lyft
provider_slug: lyft
schema_file: json-schema/lyft-ride-type-schema.json
slug: lyft-ride-type
source_filename: lyft-ride-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://lyft.com/schemas/lyft/ride-type.json\",\n  \"title\": \"Lyft Ride Type\",\n  \"description\": \"A Lyft ride type representing an available category of ride at a given location, including pricing details and passenger capacity.\",\n  \"type\": \"object\",\n  \"required\": [\"ride_type\", \"display_name\"],\n  \"properties\": {\n    \"ride_type\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the ride type.\",\n      \"enum\": [\"lyft\", \"lyft_line\", \"lyft_plus\", \"lyft_premier\", \"lyft_lux\", \"lyft_luxsuv\"]\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the ride type.\"\n    },\n    \"seats\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of passenger seats available for this ride type.\",\n      \"minimum\": 1,\n      \"maximum\": 10\n    },\n    \"image_url\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to an image representing the ride type.\"\n    },\n    \"pricing_details\": {\n      \"$ref\": \"#/$defs/PricingDetails\",\n      \"description\": \"Pricing breakdown for this ride type.\"\n    }\n  },\n  \"$defs\": {\n    \"PricingDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Pricing breakdown for a ride type. All monetary amounts are in the smallest denomination of the currency (e.g., cents for USD).\",\n      \"properties\": {\n        \"base_charge\": {\n          \"type\": \"integer\",\n          \"description\": \"Base fare amount in the smallest currency denomination.\",\n          \"minimum\": 0\n        },\n        \"cost_per_mile\": {\n          \"type\": \"integer\",\n          \"description\": \"Per-mile charge in the smallest currency denomination.\",\n          \"minimum\": 0\n        },\n        \"cost_per_minute\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"Per-minute charge in the smallest currency denomination.\",\n          \"minimum\": 0\n        },\n        \"cost_minimum\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum fare amount in the smallest currency denomination.\",\n          \"minimum\": 0\n        },\n        \"trust_and_service\": {\n          \"type\": \"integer\",\n          \"description\": \"Trust and service fee in the smallest currency denomination.\",\n          \"minimum\": 0\n        },\n        \"cancel_penalty_amount\": {\n          \"type\": \"integer\",\n          \"description\": \"Cancellation penalty amount in the smallest currency denomination.\",\n          \"minimum\": 0\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/json-schema/lyft-ride-type-schema.json
tags: []
title: Lyft Ride Type
---
