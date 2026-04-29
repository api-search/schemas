---
description: Location schema from Avalara API
layout: schema
name: Location
properties_list:
- description: PCode for jurisdiction
  name: pcd
  type: integer
- description: Country ISO code
  name: ctry
  type: string
- description: State abbreviation
  name: st
  type: string
- description: County name
  name: cty
  type: string
- description: ZIP code
  name: zip
  type: string
- description: Whether to geocode the address
  name: geo
  type: boolean
- description: Street address for geocoding
  name: addr
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-location-schema.json
slug: communications-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"Location schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pcd\": {\n      \"type\": \"integer\",\n      \"description\": \"PCode for jurisdiction\"\n    },\n    \"ctry\": {\n      \"type\": \"string\",\n      \"description\": \"Country ISO code\"\n    },\n    \"st\": {\n      \"type\": \"string\",\n      \"description\": \"State abbreviation\"\n    },\n    \"cty\": {\n      \"type\": \"string\",\n      \"description\": \"County name\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code\"\n    },\n    \"geo\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to geocode the address\"\n    },\n    \"addr\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Street address for geocoding\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-location-schema.json
tags:
- Taxes
title: Location
---
