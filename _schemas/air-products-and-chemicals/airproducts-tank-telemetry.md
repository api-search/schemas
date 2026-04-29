---
description: IoT telemetry data from a remote gas storage tank
layout: schema
name: TankTelemetry
properties_list:
- description: Tank identifier
  name: tank_id
  type: string
- description: Customer account
  name: customer_id
  type: string
- description: Gas product stored
  name: product
  type: string
- description: Current fill level as percentage
  name: level_percent
  type: number
- description: Tank pressure in bar
  name: pressure_bar
  type: number
- description: Tank temperature in Celsius
  name: temperature_c
  type: number
- description: Reading timestamp
  name: timestamp
  type: string
- description: Level % at which reorder is triggered
  name: reorder_threshold
  type: number
provider_name: Air Products and Chemicals
provider_slug: air-products-and-chemicals
schema_file: json-schema/airproducts-tank-telemetry-schema.json
slug: airproducts-tank-telemetry
source_filename: airproducts-tank-telemetry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/json-schema/airproducts-tank-telemetry-schema.json\",\n  \"title\": \"TankTelemetry\",\n  \"description\": \"IoT telemetry data from a remote gas storage tank\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tank_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tank identifier\",\n      \"example\": \"TANK-PA-001\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Customer account\",\n      \"example\": \"CUST-10045\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Gas product stored\",\n      \"example\": \"Liquid Nitrogen\"\n    },\n    \"level_percent\": {\n      \"type\": \"number\",\n      \"description\": \"Current fill level as percentage\",\n      \"example\": 72.5\n    },\n    \"pressure_bar\": {\n    \
  \  \"type\": \"number\",\n      \"description\": \"Tank pressure in bar\",\n      \"example\": 8.2\n    },\n    \"temperature_c\": {\n      \"type\": \"number\",\n      \"description\": \"Tank temperature in Celsius\",\n      \"example\": -196.0\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Reading timestamp\",\n      \"example\": \"2025-04-19T10:30:00Z\"\n    },\n    \"reorder_threshold\": {\n      \"type\": \"number\",\n      \"description\": \"Level % at which reorder is triggered\",\n      \"example\": 25.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-products-and-chemicals/refs/heads/main/json-schema/airproducts-tank-telemetry-schema.json
tags:
- Industrial Gases
- Chemicals
- Energy
- Manufacturing
- Hydrogen
- Enterprise
title: TankTelemetry
---
