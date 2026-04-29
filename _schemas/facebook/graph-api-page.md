---
description: A Facebook Page.
layout: schema
name: Page
properties_list:
- description: The page ID.
  name: id
  type: string
- description: The page name.
  name: name
  type: string
- description: Page category.
  name: category
  type: string
- description: Number of page fans.
  name: fan_count
  type: integer
- description: Page description.
  name: about
  type: string
- description: Page website URL.
  name: website
  type: string
- description: URL to the Facebook Page.
  name: link
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/graph-api-page-schema.json
slug: graph-api-page
source_filename: graph-api-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/graph-api-page-schema.json\",\n  \"title\": \"Page\",\n  \"description\": \"A Facebook Page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"The page ID.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"The page name.\" },\n    \"category\": { \"type\": \"string\", \"description\": \"Page category.\" },\n    \"fan_count\": { \"type\": \"integer\", \"description\": \"Number of page fans.\" },\n    \"about\": { \"type\": \"string\", \"description\": \"Page description.\" },\n    \"website\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Page website URL.\" },\n    \"link\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL to the Facebook Page.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/graph-api-page-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: Page
---
