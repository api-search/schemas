---
description: A pricing tier for a service.
layout: schema
name: Price
properties_list:
- description: Unique identifier for this price record.
  name: id
  type: integer
- description: Member type this price applies to (internal, external, collaborator).
  name: member_type
  type: string
- description: Price amount.
  name: amount
  type: number
- description: Currency code (ISO 4217).
  name: currency
  type: string
- description: Unit of measurement for the price.
  name: unit
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-price-schema.json
slug: ilab-operations-api-price
source_filename: ilab-operations-api-price-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-price-schema.json\",\n  \"title\": \"Price\",\n  \"description\": \"A pricing tier for a service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for this price record.\",\n      \"example\": 66\n    },\n    \"member_type\": {\n      \"type\": \"string\",\n      \"description\": \"Member type this price applies to (internal, external, collaborator).\",\n      \"enum\": [\n        \"internal\",\n        \"external\",\n        \"collaborator\"\n      ],\n      \"example\": \"internal\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Price amount.\",\n      \"example\": 150.0\n    },\n    \"currency\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Currency code (ISO 4217).\",\n      \"example\": \"USD\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement for the price.\",\n      \"example\": \"per_sample\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-price-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Price
---
