---
description: User schema from Instagram Graph API
layout: schema
name: User
properties_list:
- description: App-scoped user ID.
  name: id
  type: string
- description: Instagram username.
  name: username
  type: string
- description: Profile name.
  name: name
  type: string
- description: Profile bio text.
  name: biography
  type: string
- description: Website URL from profile.
  name: website
  type: string
- description: Profile picture URL.
  name: profile_picture_url
  type: string
- description: Total followers.
  name: followers_count
  type: integer
- description: Total accounts followed.
  name: follows_count
  type: integer
- description: Total published media.
  name: media_count
  type: integer
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-user-schema.json
slug: instagram-graph-api-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"User schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"App-scoped user ID.\",\n      \"example\": \"17841400123456789\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Instagram username.\",\n      \"example\": \"examplebusiness\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Profile name.\",\n      \"example\": \"Example Business\"\n    },\n    \"biography\": {\n      \"type\": \"string\",\n      \"description\": \"Profile bio text.\",\n      \"example\": \"Official account for Example Business.\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Website URL from profile.\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"profile_picture_url\": {\n      \"type\": \"string\",\n      \"description\": \"Profile picture URL.\",\n      \"example\": \"https://scontent.cdninstagram.com/example.jpg\"\n    },\n    \"followers_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total followers.\",\n      \"example\": 15000\n    },\n    \"follows_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total accounts followed.\",\n      \"example\": 500\n    },\n    \"media_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total published media.\",\n      \"example\": 342\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-user-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: User
---
