---
description: ''
layout: schema
name: ExperienceHost
properties_list:
- description: The unique identifier of the experience host.
  name: id
  type: string
- description: The display name of the host.
  name: name
  type: string
- description: A short biography of the host.
  name: bio
  type: string
- description: The URL of the host profile picture.
  name: profile_picture_url
  type: string
- description: Whether the host has Superhost status.
  name: superhost
  type: boolean
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-experience-host-schema.json
slug: airbnb-experience-host
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-host-schema.json\",\n  \"title\": \"ExperienceHost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the experience host.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the host.\"\n    },\n    \"bio\": {\n      \"type\": \"string\",\n      \"description\": \"A short biography of the host.\"\n    },\n    \"profile_picture_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the host profile picture.\"\n    },\n    \"superhost\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the host has Superhost status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-host-schema.json
tags: []
title: ExperienceHost
---
