---
description: ''
layout: schema
name: Guest
properties_list:
- description: The unique identifier of the guest.
  name: id
  type: string
- description: The first name of the guest.
  name: first_name
  type: string
- description: The last name of the guest.
  name: last_name
  type: string
- description: The phone number of the guest, available after booking is confirmed.
  name: phone
  type: string
- description: The URL of the guest profile picture.
  name: profile_picture_url
  type: string
- description: Whether the guest has completed identity verification.
  name: verified
  type: boolean
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-guest-schema.json
slug: airbnb-guest
source_filename: airbnb-guest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-guest-schema.json\",\n  \"title\": \"Guest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the guest.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the guest.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the guest.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the guest, available after booking is confirmed.\"\n    },\n    \"profile_picture_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the guest profile picture.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether the guest has completed identity verification.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-guest-schema.json
tags: []
title: Guest
---
