---
description: User schema from 1Factory API
layout: schema
name: User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: integer
- description: Full name of the user.
  name: name
  type: string
- description: Email address of the user.
  name: email
  type: string
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-user-schema.json
slug: 1factory-user
source_filename: 1factory-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"User schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"nullable\": false,\n      \"description\": \"Unique identifier for the user.\",\n      \"example\": 5127\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"maxLength\": 255,\n      \"description\": \"Full name of the user.\",\n      \"example\": \"John Doe\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"format\": \"email\",\n      \"maxLength\": 255,\n      \"description\": \"Email address of the user.\",\n      \"example\": \"jon.doe@1factory.com\"\n    }\n  },\n  \"required\": [\n    \"id\"\
  ,\n    \"name\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-user-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: User
---
