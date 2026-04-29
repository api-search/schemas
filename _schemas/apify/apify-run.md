---
description: An Apify Actor run execution.
layout: schema
name: Run
properties_list:
- description: Run ID.
  name: id
  type: string
- description: Actor ID.
  name: actId
  type: string
- description: Run status.
  name: status
  type: string
- description: Run start time.
  name: startedAt
  type: string
- description: Run finish time.
  name: finishedAt
  type: string
- description: ID of the default dataset for this run.
  name: defaultDatasetId
  type: string
provider_name: Apify
provider_slug: apify
schema_file: json-schema/apify-run-schema.json
slug: apify-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-run-schema.json\",\n  \"title\": \"Run\",\n  \"description\": \"An Apify Actor run execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Run ID.\",\n      \"example\": \"HG7ML7M8z78YcAPEB\"\n    },\n    \"actId\": {\n      \"type\": \"string\",\n      \"description\": \"Actor ID.\",\n      \"example\": \"mTD6bTz2HCjSQHeBn\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"READY\",\n        \"RUNNING\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"ABORTED\",\n        \"TIMED-OUT\"\n      ],\n      \"description\": \"Run status.\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Run start time.\"\n    },\n    \"finishedAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Run finish time.\"\n    },\n    \"defaultDatasetId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the default dataset for this run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apify/refs/heads/main/json-schema/apify-run-schema.json
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
title: Run
---
