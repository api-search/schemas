---
description: Single city record returned by the AirLabs Cities Database API.
layout: schema
name: AirLabs City
properties_list:
- description: English name of the city.
  name: name
  type: string
- description: IATA metropolitan area code.
  name: city_code
  type: string
- description: UN/LOCODE for the city.
  name: un_code
  type: string
- description: SEO-friendly slug.
  name: slug
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country_code
  type: string
- description: Latitude in decimal degrees.
  name: lat
  type: number
- description: Longitude in decimal degrees.
  name: lng
  type: number
- description: Elevation in meters.
  name: elevation
  type: integer
- description: IANA timezone identifier.
  name: timezone
  type: string
- description: Population count.
  name: population
  type: integer
- description: Wikipedia article URL.
  name: wikipedia
  type: string
- description: Multilingual city names keyed by ISO 639-1 language code.
  name: names
  type: object
provider_name: Cities Database API
provider_slug: cities-database-api
schema_file: json-schema/cities-database-api-city-schema.json
slug: cities-database-api-city
source_filename: cities-database-api-city-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cities-database-api/main/json-schema/cities-database-api-city-schema.json\",\n  \"title\": \"AirLabs City\",\n  \"description\": \"Single city record returned by the AirLabs Cities Database API.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"city_code\", \"country_code\", \"lat\", \"lng\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"English name of the city.\"\n    },\n    \"city_code\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"IATA metropolitan area code.\"\n    },\n    \"un_code\": {\n      \"type\": \"string\",\n      \"description\": \"UN/LOCODE for the city.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"SEO-friendly slug.\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"\
  pattern\": \"^[A-Z]{2}$\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\"\n    },\n    \"lat\": {\n      \"type\": \"number\",\n      \"minimum\": -90,\n      \"maximum\": 90,\n      \"description\": \"Latitude in decimal degrees.\"\n    },\n    \"lng\": {\n      \"type\": \"number\",\n      \"minimum\": -180,\n      \"maximum\": 180,\n      \"description\": \"Longitude in decimal degrees.\"\n    },\n    \"elevation\": {\n      \"type\": \"integer\",\n      \"description\": \"Elevation in meters.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"IANA timezone identifier.\"\n    },\n    \"population\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Population count.\"\n    },\n    \"wikipedia\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Wikipedia article URL.\"\n    },\n    \"names\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\"type\": \"\
  string\"},\n      \"description\": \"Multilingual city names keyed by ISO 639-1 language code.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cities-database-api/refs/heads/main/json-schema/cities-database-api-city-schema.json
tags:
- Cities
- Data
- Geography
- Locations
- Reference Data
- Travel
title: AirLabs City
---
