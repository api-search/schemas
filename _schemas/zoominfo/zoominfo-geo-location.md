---
description: ''
layout: schema
name: GeoLocation
properties_list:
- description: ''
  name: location_long
  type: number
- description: ''
  name: location_lat
  type: number
- description: ''
  name: country_code
  type: string
- description: ''
  name: province
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-geo-location-schema.json
slug: zoominfo-geo-location
source_filename: zoominfo-geo-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"location_long\": {\n      \"type\": \"number\",\n      \"example\": 75.5\n    },\n    \"location_lat\": {\n      \"type\": \"number\",\n      \"example\": 75.5\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"province\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"location_long\",\n    \"location_lat\",\n    \"country_code\",\n    \"province\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeoLocation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-geo-location-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: GeoLocation
---
