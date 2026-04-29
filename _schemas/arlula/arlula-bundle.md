---
description: An imagery bundle option with specific products and pricing.
layout: schema
name: Bundle
properties_list:
- description: Bundle key used when placing orders.
  name: key
  type: string
- description: Bundle display name.
  name: name
  type: string
- description: Bundle price.
  name: price
  type: number
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-bundle-schema.json
slug: arlula-bundle
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/bundle.json\",\n  \"title\": \"Bundle\",\n  \"description\": \"An imagery bundle option with specific products and pricing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle key used when placing orders.\",\n      \"examples\": [\n        \"bundle-basic\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Bundle display name.\",\n      \"examples\": [\n        \"Basic Bundle\"\n      ]\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Bundle price.\",\n      \"examples\": [\n        150.0\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-bundle-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Bundle
---
