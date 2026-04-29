---
description: An Apify key-value store for persistent data.
layout: schema
name: KeyValueStore
properties_list:
- description: Store ID.
  name: id
  type: string
- description: Store name.
  name: name
  type: string
provider_name: Apify
provider_slug: apify
schema_file: json-schema/apify-key-value-store-schema.json
slug: apify-key-value-store
source_filename: apify-key-value-store-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-key-value-store-schema.json\",\n  \"title\": \"KeyValueStore\",\n  \"description\": \"An Apify key-value store for persistent data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Store ID.\",\n      \"example\": \"WkzbQMuFYuamGv3YQ\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Store name.\",\n      \"example\": \"my-store\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-key-value-store-schema.json
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
title: KeyValueStore
---
