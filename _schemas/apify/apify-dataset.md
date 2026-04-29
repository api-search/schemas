---
description: An Apify dataset for storing structured scraping results.
layout: schema
name: Dataset
properties_list:
- description: Dataset ID.
  name: id
  type: string
- description: Dataset name.
  name: name
  type: string
- description: Number of items in the dataset.
  name: itemCount
  type: integer
provider_name: Apify
provider_slug: apify
schema_file: json-schema/apify-dataset-schema.json
slug: apify-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"An Apify dataset for storing structured scraping results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset ID.\",\n      \"example\": \"s5gkMuSS6Tsh4iOLF\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name.\",\n      \"example\": \"my-dataset\"\n    },\n    \"itemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of items in the dataset.\",\n      \"example\": 150\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-dataset-schema.json
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
title: Dataset
---
