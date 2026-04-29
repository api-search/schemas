---
description: ''
layout: schema
name: AcquisitionDate
properties_list:
- description: Defines the acquisition start date. The parameter can be set at any time. Note that if the parameter is set in the past, the value is replaced by the current date
  name: startDate
  type: string
- description: Defines the acquisition end date
  name: endDate
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-acquisition-date-schema.json
slug: oneatlas-acquisition-date
source_filename: oneatlas-acquisition-date-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-acquisition-date-schema.json\",\n  \"title\": \"AcquisitionDate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"datetime\",\n      \"pattern\": \"^yyyy-MM-dd'T'HH:mm:ss.SSS'Z$\",\n      \"description\": \"Defines the acquisition start date. The parameter can be set at any time. Note that if the parameter is set in the past, the value is replaced by the current date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"datetime\",\n      \"pattern\": \"^yyyy-MM-dd'T'HH:mm:ss.SSS'Z$\",\n      \"description\": \"Defines the acquisition end date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-acquisition-date-schema.json
tags:
- Imagery
- Satellites
title: AcquisitionDate
---
