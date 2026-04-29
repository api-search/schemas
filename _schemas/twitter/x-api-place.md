---
description: Place schema from X API v2
layout: schema
name: Place
properties_list:
- description: ''
  name: contained_within
  type: array
- description: The full name of the county in which this place exists.
  name: country
  type: string
- description: A two-letter ISO 3166-1 alpha-2 country code.
  name: country_code
  type: string
- description: The full name of this place.
  name: full_name
  type: string
- description: ''
  name: geo
  type: object
- description: The identifier for this place.
  name: id
  type: string
- description: The human readable name of this place.
  name: name
  type: string
- description: ''
  name: place_type
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-place-schema.json
slug: x-api-place
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-place-schema.json\",\n  \"title\": \"Place\",\n  \"description\": \"Place schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contained_within\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PlaceId\"\n      }\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the county in which this place exists.\",\n      \"example\": \"United States\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"A two-letter ISO 3166-1 alpha-2 country code.\",\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"example\": \"US\"\n    },\n    \"full_name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of this place.\",\n      \"example\"\
  : \"Lakewood, CO\"\n    },\n    \"geo\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\",\n        \"bbox\",\n        \"properties\"\n      ],\n      \"properties\": {\n        \"bbox\": {\n          \"type\": \"array\",\n          \"minItems\": 4,\n          \"maxItems\": 4,\n          \"items\": {\n            \"type\": \"number\",\n            \"minimum\": -180,\n            \"maximum\": 180,\n            \"format\": \"double\"\n          },\n          \"example\": [\n            -105.193475,\n            39.60973,\n            -105.053164,\n            39.761974\n          ]\n        },\n        \"geometry\": {\n          \"$ref\": \"#/components/schemas/Point\"\n        },\n        \"properties\": {\n          \"type\": \"object\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Feature\"\n          ]\n        }\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier\
  \ for this place.\",\n      \"example\": \"f7eb2fa2fea288b1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human readable name of this place.\",\n      \"example\": \"Lakewood\"\n    },\n    \"place_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"poi\",\n        \"neighborhood\",\n        \"city\",\n        \"admin\",\n        \"country\",\n        \"unknown\"\n      ],\n      \"example\": \"city\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"full_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-place-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Place
---
