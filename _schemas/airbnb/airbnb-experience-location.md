---
description: ''
layout: schema
name: ExperienceLocation
properties_list:
- description: Description of where guests should meet for the experience.
  name: meeting_point
  type: string
- description: The city where the experience takes place.
  name: city
  type: string
- description: The state or province where the experience takes place.
  name: state
  type: string
- description: The ISO 3166-1 alpha-2 country code.
  name: country
  type: string
- description: The latitude coordinate of the meeting point.
  name: latitude
  type: number
- description: The longitude coordinate of the meeting point.
  name: longitude
  type: number
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-experience-location-schema.json
slug: airbnb-experience-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-location-schema.json\",\n  \"title\": \"ExperienceLocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meeting_point\": {\n      \"type\": \"string\",\n      \"description\": \"Description of where guests should meet for the experience.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city where the experience takes place.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province where the experience takes place.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 3166-1 alpha-2 country code.\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The latitude coordinate\
  \ of the meeting point.\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The longitude coordinate of the meeting point.\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    }\n  },\n  \"required\": [\n    \"city\",\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-location-schema.json
tags: []
title: ExperienceLocation
---
