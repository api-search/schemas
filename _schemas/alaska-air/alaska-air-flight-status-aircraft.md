---
description: Aircraft information for the flight
layout: schema
name: Aircraft
properties_list:
- description: Aircraft type/model
  name: type
  type: string
- description: Aircraft tail number (registration)
  name: tailNumber
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-flight-status-aircraft-schema.json
slug: alaska-air-flight-status-aircraft
source_filename: alaska-air-flight-status-aircraft-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-aircraft-schema.json\",\n  \"title\": \"Aircraft\",\n  \"description\": \"Aircraft information for the flight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Aircraft type/model\",\n      \"example\": \"Boeing 737-900ER\"\n    },\n    \"tailNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Aircraft tail number (registration)\",\n      \"example\": \"N491AS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-flight-status-aircraft-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Aircraft
---
