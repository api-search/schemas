---
description: A documented police brutality incident from the 2020 George Floyd protests
layout: schema
name: Incident
properties_list:
- description: 'Unique identifier for the incident (format: state-city-number)'
  name: id
  type: string
- description: Brief title or summary of the incident
  name: name
  type: string
- description: Detailed description of what occurred during the incident
  name: description
  type: string
- description: Date the incident occurred (ISO 8601 format)
  name: date
  type: string
- description: Human-readable date description
  name: date_text
  type: string
- description: US state abbreviation where the incident occurred
  name: state
  type: string
- description: City where the incident occurred
  name: city
  type: string
- description: Latitude and longitude coordinates of the incident location
  name: geolocation
  type: string
- description: Categorical tags describing the type of incident or force used
  name: tags
  type: array
- description: Source URLs documenting or referencing the incident
  name: links
  type: array
- description: Direct link to edit this incident record on GitHub
  name: edit_at
  type: string
provider_name: 2020 Police Brutality
provider_slug: 2020-police-brutality
schema_file: json-schema/2020-police-brutality-incident-schema.json
slug: 2020-police-brutality-incident
source_filename: 2020-police-brutality-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/2020-police-brutality/refs/heads/main/json-schema/2020-police-brutality-incident-schema.json\",\n  \"title\": \"Incident\",\n  \"description\": \"A documented police brutality incident from the 2020 George Floyd protests\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the incident (format: state-city-number)\",\n      \"example\": \"nm-albuquerque-1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Brief title or summary of the incident\",\n      \"example\": \"Student journalist struck by foam bullet\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of what occurred during the incident\",\n      \"example\": \"A student journalist was struck by a foam bullet while\
  \ covering protests near downtown.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the incident occurred (ISO 8601 format)\",\n      \"example\": \"2020-06-01\"\n    },\n    \"date_text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable date description\",\n      \"example\": \"June 1st\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state abbreviation where the incident occurred\",\n      \"example\": \"NM\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the incident occurred\",\n      \"example\": \"Albuquerque\"\n    },\n    \"geolocation\": {\n      \"type\": \"string\",\n      \"description\": \"Latitude and longitude coordinates of the incident location\",\n      \"example\": \"35.0844,-106.6504\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Categorical tags describing the type\
  \ of incident or force used\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"foam-bullet\",\n        \"journalist\",\n        \"protester\"\n      ]\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"Source URLs documenting or referencing the incident\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"example\": [\n        \"https://example.com/news-article\",\n        \"https://twitter.com/example/status/123456\"\n      ]\n    },\n    \"edit_at\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Direct link to edit this incident record on GitHub\",\n      \"example\": \"https://github.com/2020PB/police-brutality/edit/main/reports/New%20Mexico.md\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/2020-police-brutality/refs/heads/main/json-schema/2020-police-brutality-incident-schema.json
tags:
- Brutality
- Civil Rights
- Policing
- Public Data
title: Incident
---
