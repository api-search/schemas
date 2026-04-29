---
description: ''
layout: schema
name: GetBrokerStrategiesResponse
properties_list:
- description: List of available strategy names
  name: strategies
  type: array
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-get-broker-strategies-response-schema.json
slug: bloomberg-emsx-get-broker-strategies-response
source_filename: bloomberg-emsx-get-broker-strategies-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetBrokerStrategiesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"strategies\": {\n      \"type\": \"array\",\n      \"description\": \"List of available strategy names\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-get-broker-strategies-response-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GetBrokerStrategiesResponse
---
