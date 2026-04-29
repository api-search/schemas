---
description: ''
layout: schema
name: GeoLocation
properties_list:
- description: ''
  name: city
  type: '[''string'', ''null'']'
- description: ''
  name: state
  type: '[''string'', ''null'']'
- description: ''
  name: stateCode
  type: '[''string'', ''null'']'
- description: ''
  name: country
  type: '[''string'', ''null'']'
- description: ''
  name: countryCode
  type: '[''string'', ''null'']'
- description: ''
  name: lat
  type: '[''number'', ''null'']'
- description: ''
  name: lng
  type: '[''number'', ''null'']'
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-geo-location-schema.json
slug: hunter-geo-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeoLocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"state\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"stateCode\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"country\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"countryCode\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"lat\": {\n      \"type\": \"['number', 'null']\"\n    },\n    \"lng\": {\n      \"type\": \"['number', 'null']\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-geo-location-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: GeoLocation
---
