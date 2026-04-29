---
description: ''
layout: schema
name: ExperiencePricing
properties_list:
- description: The price per guest in the specified currency.
  name: price_per_person
  type: number
- description: The ISO 4217 currency code for pricing.
  name: currency
  type: string
- description: Optional group discount configuration.
  name: group_discount
  type: object
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-experience-pricing-schema.json
slug: airbnb-experience-pricing
source_filename: airbnb-experience-pricing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-pricing-schema.json\",\n  \"title\": \"ExperiencePricing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"price_per_person\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The price per guest in the specified currency.\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for pricing.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"group_discount\": {\n      \"type\": \"object\",\n      \"description\": \"Optional group discount configuration.\",\n      \"properties\": {\n        \"min_guests\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum number of guests to qualify for the group discount.\",\n          \"minimum\": 2\n        },\n\
  \        \"discount_percent\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage discount applied for group bookings.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"price_per_person\",\n    \"currency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-pricing-schema.json
tags: []
title: ExperiencePricing
---
