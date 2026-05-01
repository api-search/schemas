---
description: A business location managed through the Google Business Profile API.
layout: schema
name: Google Business Profile Location
properties_list:
- description: Google identifier for this location.
  name: name
  type: string
- description: The name of the business location.
  name: locationName
  type: string
- description: Primary phone number of the business.
  name: primaryPhone
  type: string
- description: Physical address of the business.
  name: address
  type: object
- description: Primary business category.
  name: primaryCategory
  type: object
- description: URL for the business website.
  name: websiteUrl
  type: string
- description: Regular business hours.
  name: regularHours
  type: object
- description: State of the location.
  name: locationState
  type: object
- description: Additional metadata for the location.
  name: metadata
  type: object
provider_name: Google Business Profile
provider_slug: google-business-profile
schema_file: json-schema/Location.json
slug: Location
source_filename: Location.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"Location.json\",\n  \"title\": \"Google Business Profile Location\",\n  \"description\": \"A business location managed through the Google Business Profile API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Google identifier for this location.\"\n    },\n    \"locationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the business location.\"\n    },\n    \"primaryPhone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number of the business.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address of the business.\",\n      \"properties\": {\n        \"addressLines\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"locality\": {\n          \"type\"\
  : \"string\"\n        },\n        \"administrativeArea\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"regionCode\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"primaryCategory\": {\n      \"type\": \"object\",\n      \"description\": \"Primary business category.\",\n      \"properties\": {\n        \"displayName\": {\n          \"type\": \"string\"\n        },\n        \"categoryId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"websiteUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the business website.\"\n    },\n    \"regularHours\": {\n      \"type\": \"object\",\n      \"description\": \"Regular business hours.\"\n    },\n    \"locationState\": {\n      \"type\": \"object\",\n      \"description\": \"State of the location.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Additional metadata for the location.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-business-profile/refs/heads/main/json-schema/Location.json
tags:
- Business Profiles
- Google
- Local Business
- Locations
- Reviews
title: Google Business Profile Location
---
