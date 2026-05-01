---
description: A user-contributed tip about a Foursquare place.
layout: schema
name: FoursquareTip
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: text
  type: string
provider_name: Foursquare
provider_slug: foursquare
schema_file: json-schema/foursquare-tip.json
slug: foursquare-tip
source_filename: foursquare-tip.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/json-schema/foursquare-tip.json\",\n  \"title\": \"FoursquareTip\",\n  \"description\": \"A user-contributed tip about a Foursquare place.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"text\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"text\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/json-schema/foursquare-tip.json
tags:
- Locations
- Places
- Geocoding
- Recommendations
- Reviews
- Movement
title: FoursquareTip
---
