---
description: ''
layout: schema
name: ExperiencePhoto
properties_list:
- description: The unique identifier of the photo.
  name: id
  type: string
- description: The URL where the photo is hosted.
  name: url
  type: string
- description: A caption describing the photo.
  name: caption
  type: string
- description: The display position of the photo.
  name: sort_order
  type: integer
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-experience-photo-schema.json
slug: airbnb-experience-photo
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-photo-schema.json\",\n  \"title\": \"ExperiencePhoto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the photo.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL where the photo is hosted.\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"A caption describing the photo.\"\n    },\n    \"sort_order\": {\n      \"type\": \"integer\",\n      \"description\": \"The display position of the photo.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-photo-schema.json
tags: []
title: ExperiencePhoto
---
