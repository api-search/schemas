---
description: UserLocation schema from Google Analytics API
layout: schema
name: UserLocation
properties_list:
- description: City name.
  name: city
  type: string
- description: Region identifier.
  name: region_id
  type: string
- description: Country identifier.
  name: country_id
  type: string
- description: Subcontinent identifier.
  name: subcontinent_id
  type: string
- description: Continent identifier.
  name: continent_id
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/measurement-protocol-user-location-schema.json
slug: measurement-protocol-user-location
source_filename: measurement-protocol-user-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-user-location-schema.json\",\n  \"title\": \"UserLocation\",\n  \"description\": \"UserLocation schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name.\",\n      \"example\": \"example_value\"\n    },\n    \"region_id\": {\n      \"type\": \"string\",\n      \"description\": \"Region identifier.\",\n      \"example\": \"123456\"\n    },\n    \"country_id\": {\n      \"type\": \"string\",\n      \"description\": \"Country identifier.\",\n      \"example\": \"123456\"\n    },\n    \"subcontinent_id\": {\n      \"type\": \"string\",\n      \"description\": \"Subcontinent identifier.\",\n      \"example\": \"123456\"\n    },\n    \"continent_id\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Continent identifier.\",\n      \"example\": \"123456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-user-location-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: UserLocation
---
