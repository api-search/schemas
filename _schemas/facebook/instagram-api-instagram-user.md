---
description: An Instagram Business or Creator account.
layout: schema
name: InstagramUser
properties_list:
- description: Instagram user ID.
  name: id
  type: string
- description: Instagram username.
  name: username
  type: string
- description: Display name.
  name: name
  type: string
- description: Account biography.
  name: biography
  type: string
- description: Number of followers.
  name: followers_count
  type: integer
- description: Number of accounts followed.
  name: follows_count
  type: integer
- description: Number of media posts.
  name: media_count
  type: integer
- description: Profile picture URL.
  name: profile_picture_url
  type: string
- description: Website URL.
  name: website
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/instagram-api-instagram-user-schema.json
slug: instagram-api-instagram-user
source_filename: instagram-api-instagram-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/instagram-api-instagram-user-schema.json\",\n  \"title\": \"InstagramUser\",\n  \"description\": \"An Instagram Business or Creator account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Instagram user ID.\" },\n    \"username\": { \"type\": \"string\", \"description\": \"Instagram username.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Display name.\" },\n    \"biography\": { \"type\": \"string\", \"description\": \"Account biography.\" },\n    \"followers_count\": { \"type\": \"integer\", \"description\": \"Number of followers.\" },\n    \"follows_count\": { \"type\": \"integer\", \"description\": \"Number of accounts followed.\" },\n    \"media_count\": { \"type\": \"integer\", \"description\": \"Number of media posts.\" },\n    \"\
  profile_picture_url\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Profile picture URL.\" },\n    \"website\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Website URL.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/instagram-api-instagram-user-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: InstagramUser
---
