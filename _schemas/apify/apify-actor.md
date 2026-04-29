---
description: An Apify Actor for web scraping and automation.
layout: schema
name: Actor
properties_list:
- description: Actor ID.
  name: id
  type: string
- description: Actor name.
  name: name
  type: string
- description: Owner username.
  name: username
  type: string
- description: Display title.
  name: title
  type: string
- description: Actor description.
  name: description
  type: string
provider_name: Apify
provider_slug: apify
schema_file: json-schema/apify-actor-schema.json
slug: apify-actor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-actor-schema.json\",\n  \"title\": \"Actor\",\n  \"description\": \"An Apify Actor for web scraping and automation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Actor ID.\",\n      \"example\": \"mTD6bTz2HCjSQHeBn\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Actor name.\",\n      \"example\": \"web-scraper\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Owner username.\",\n      \"example\": \"apify\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title.\",\n      \"example\": \"Web Scraper\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Actor description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-actor-schema.json
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
title: Actor
---
