---
description: A city record from the SAM.gov Public Location Services API
layout: schema
name: SAM.gov City
properties_list:
- description: Unique city code identifier in SAM.gov
  name: cityCode
  type: string
- description: Full city name
  name: cityName
  type: string
- description: State or province code
  name: stateCode
  type: string
- description: Full state or province name
  name: stateName
  type: string
- description: County code
  name: countyCode
  type: string
- description: County name
  name: countyName
  type: string
- description: ISO 3166-1 alpha-2 country code (e.g. US)
  name: countryCode
  type: string
- description: Full country name
  name: countryName
  type: string
- description: Whether this city record is active (Y) or inactive (N)
  name: activeInd
  type: string
provider_name: SAM.gov
provider_slug: sam.gov
schema_file: json-schema/sam-gov-city-schema.json
slug: sam-gov-city
source_filename: sam-gov-city-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sam.gov/json-schema/sam-gov-city-schema.json\",\n  \"title\": \"SAM.gov City\",\n  \"description\": \"A city record from the SAM.gov Public Location Services API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cityCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique city code identifier in SAM.gov\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"Full city name\"\n    },\n    \"stateCode\": {\n      \"type\": \"string\",\n      \"description\": \"State or province code\"\n    },\n    \"stateName\": {\n      \"type\": \"string\",\n      \"description\": \"Full state or province name\"\n    },\n    \"countyCode\": {\n      \"type\": \"string\",\n      \"description\": \"County code\"\n    },\n    \"countyName\": {\n      \"type\": \"string\",\n      \"description\": \"County name\"\n    },\n    \"countryCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code (e.g. US)\"\n    },\n    \"countryName\": {\n      \"type\": \"string\",\n      \"description\": \"Full country name\"\n    },\n    \"activeInd\": {\n      \"type\": \"string\",\n      \"enum\": [\"Y\", \"N\"],\n      \"description\": \"Whether this city record is active (Y) or inactive (N)\"\n    }\n  },\n  \"required\": [\"cityCode\", \"cityName\", \"countryCode\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sam.gov/refs/heads/main/json-schema/sam-gov-city-schema.json
tags:
- Federal Government
- Procurement
- Contracts
- Entity Management
- Location Services
- GSA
title: SAM.gov City
---
