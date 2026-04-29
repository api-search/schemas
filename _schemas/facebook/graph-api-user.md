---
description: A Facebook user profile.
layout: schema
name: User
properties_list:
- description: The user ID.
  name: id
  type: string
- description: The user's full name.
  name: name
  type: string
- description: The user's email address.
  name: email
  type: string
- description: First name.
  name: first_name
  type: string
- description: Last name.
  name: last_name
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/graph-api-user-schema.json
slug: graph-api-user
source_filename: graph-api-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/graph-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A Facebook user profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"The user ID.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"The user's full name.\" },\n    \"email\": { \"type\": \"string\", \"format\": \"email\", \"description\": \"The user's email address.\" },\n    \"first_name\": { \"type\": \"string\", \"description\": \"First name.\" },\n    \"last_name\": { \"type\": \"string\", \"description\": \"Last name.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/graph-api-user-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: User
---
