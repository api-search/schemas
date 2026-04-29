---
description: Geographic targeting configuration.
layout: schema
name: GeoTargeting
properties_list:
- description: Countries to target.
  name: countries
  type: array
- description: Regions to target.
  name: regions
  type: array
- description: Cities to target.
  name: cities
  type: array
- description: Metros to target.
  name: metros
  type: array
- description: Postal codes to target.
  name: postalCodes
  type: array
- description: Whether to exclude the specified geographic locations.
  name: excludeCountries
  type: boolean
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-geo-targeting-schema.json
slug: google-campaign-manager-geo-targeting
source_filename: google-campaign-manager-geo-targeting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeoTargeting\",\n  \"type\": \"object\",\n  \"description\": \"Geographic targeting configuration.\",\n  \"properties\": {\n    \"countries\": {\n      \"type\": \"array\",\n      \"description\": \"Countries to target.\"\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"description\": \"Regions to target.\"\n    },\n    \"cities\": {\n      \"type\": \"array\",\n      \"description\": \"Cities to target.\"\n    },\n    \"metros\": {\n      \"type\": \"array\",\n      \"description\": \"Metros to target.\"\n    },\n    \"postalCodes\": {\n      \"type\": \"array\",\n      \"description\": \"Postal codes to target.\"\n    },\n    \"excludeCountries\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to exclude the specified geographic locations.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-geo-targeting-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: GeoTargeting
---
