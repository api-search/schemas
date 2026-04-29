---
description: ''
layout: schema
name: Spectrum Enterprise Serviceability
properties_list:
- description: ''
  name: address
  type: object
- description: ''
  name: isServiceable
  type: boolean
- description: ''
  name: availableProducts
  type: array
provider_name: Charter Communications
provider_slug: charter-communications
schema_file: json-schema/charter-communications-serviceability-schema.json
slug: charter-communications-serviceability
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://enterprise.spectrum.com/schemas/serviceability.json\",\n  \"title\": \"Spectrum Enterprise Serviceability\",\n  \"type\": \"object\",\n  \"required\": [\"address\", \"isServiceable\"],\n  \"properties\": {\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" }\n      }\n    },\n    \"isServiceable\": { \"type\": \"boolean\" },\n    \"availableProducts\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charter-communications/refs/heads/main/json-schema/charter-communications-serviceability-schema.json
tags:
- Broadband
- Cable
- CAMARA
- Enterprise
- Network as a Service
- NaaS
- Spectrum
- Telecommunications
- Ticketing
title: Spectrum Enterprise Serviceability
---
