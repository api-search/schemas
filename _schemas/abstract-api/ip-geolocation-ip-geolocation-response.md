---
description: IP geolocation response data
layout: schema
name: IPGeolocationResponse
properties_list:
- description: The queried IP address
  name: ip_address
  type: string
- description: City name
  name: city
  type: string
- description: Geonames ID for the city
  name: city_geoname_id
  type: integer
- description: Region or state name
  name: region
  type: string
- description: ISO region code
  name: region_iso_code
  type: string
- description: Geonames ID for the region
  name: region_geoname_id
  type: integer
- description: Postal or ZIP code
  name: postal_code
  type: string
- description: Country name
  name: country
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country_code
  type: string
- description: Geonames ID for the country
  name: country_geoname_id
  type: integer
- description: Whether the country is in the EU
  name: country_is_eu
  type: boolean
- description: Continent name
  name: continent
  type: string
- description: Continent code
  name: continent_code
  type: string
- description: Geonames ID for the continent
  name: continent_geoname_id
  type: integer
- description: Longitude coordinate
  name: longitude
  type: number
- description: Latitude coordinate
  name: latitude
  type: number
- description: ''
  name: security
  type: object
- description: ''
  name: timezone
  type: object
- description: ''
  name: flag
  type: object
- description: ''
  name: currency
  type: object
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-geolocation-ip-geolocation-response-schema.json
slug: ip-geolocation-ip-geolocation-response
source_filename: ip-geolocation-ip-geolocation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-ip-geolocation-response-schema.json\",\n  \"title\": \"IPGeolocationResponse\",\n  \"description\": \"IP geolocation response data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"The queried IP address\",\n      \"example\": \"8.8.8.8\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\",\n      \"example\": \"Mountain View\"\n    },\n    \"city_geoname_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Geonames ID for the city\",\n      \"example\": 5375480\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region or state name\",\n      \"example\": \"California\"\n    },\n    \"region_iso_code\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"ISO region code\",\n      \"example\": \"CA\"\n    },\n    \"region_geoname_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Geonames ID for the region\",\n      \"example\": 5332921\n    },\n    \"postal_code\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\",\n      \"example\": \"94043\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country name\",\n      \"example\": \"United States\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\",\n      \"example\": \"US\"\n    },\n    \"country_geoname_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Geonames ID for the country\",\n      \"example\": 6252001\n    },\n    \"country_is_eu\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the country is in the EU\",\n      \"example\": false\n    },\n    \"continent\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Continent name\",\n      \"example\": \"North America\"\n    },\n    \"continent_code\": {\n      \"type\": \"string\",\n      \"description\": \"Continent code\",\n      \"example\": \"NA\"\n    },\n    \"continent_geoname_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Geonames ID for the continent\",\n      \"example\": 6255149\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Longitude coordinate\",\n      \"example\": -122.0838\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Latitude coordinate\",\n      \"example\": 37.386\n    },\n    \"security\": {\n      \"$ref\": \"#/components/schemas/SecurityInfo\"\n    },\n    \"timezone\": {\n      \"$ref\": \"#/components/schemas/TimezoneInfo\"\n    },\n    \"flag\": {\n      \"$ref\": \"#/components/schemas/FlagInfo\"\n    },\n    \"currency\": {\n \
  \     \"$ref\": \"#/components/schemas/CurrencyInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-ip-geolocation-response-schema.json
tags:
- Avatars
- Company Enrichment
- Contacts
- Currencies
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
title: IPGeolocationResponse
---
