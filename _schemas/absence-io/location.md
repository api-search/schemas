---
description: An office or work location.
layout: schema
name: Location
properties_list:
- description: Unique identifier of the location.
  name: _id
  type: string
- description: Name of the location.
  name: name
  type: string
- description: Timezone identifier for this location.
  name: timezone
  type: string
- description: Country code for the location.
  name: country
  type: string
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/location-schema.json
slug: location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"An office or work location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the location.\",\n      \"example\": \"500888\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the location.\",\n      \"example\": \"HQ-SanFrancisco\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone identifier for this location.\",\n      \"example\": \"America/Los_Angeles\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code for the location.\",\n      \"example\": \"US\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/location-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: Location
---
