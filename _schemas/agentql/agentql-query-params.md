---
description: Optional configuration parameters for the query.
layout: schema
name: QueryParams
properties_list:
- description: Extraction speed mode. Fast is quicker but may miss dynamic content.
  name: mode
  type: string
- description: Milliseconds to wait for dynamic content to load before extraction.
  name: wait_for
  type: integer
- description: If true, scroll to the bottom of the page before extraction.
  name: scroll_to_bottom
  type: boolean
- description: If true, include a base64-encoded screenshot in the response.
  name: include_screenshot
  type: boolean
- description: Browser profile to use for the request.
  name: browser_profile
  type: string
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-query-params-schema.json
slug: agentql-query-params
source_filename: agentql-query-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-params-schema.json\",\n  \"title\": \"QueryParams\",\n  \"description\": \"Optional configuration parameters for the query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"fast\",\n        \"standard\"\n      ],\n      \"description\": \"Extraction speed mode. Fast is quicker but may miss dynamic content.\",\n      \"example\": \"standard\"\n    },\n    \"wait_for\": {\n      \"type\": \"integer\",\n      \"description\": \"Milliseconds to wait for dynamic content to load before extraction.\",\n      \"example\": 2000\n    },\n    \"scroll_to_bottom\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, scroll to the bottom of the page before extraction.\",\n      \"example\": false\n    },\n    \"include_screenshot\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"If true, include a base64-encoded screenshot in the response.\",\n      \"example\": false\n    },\n    \"browser_profile\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"light\",\n        \"stealth\"\n      ],\n      \"description\": \"Browser profile to use for the request.\",\n      \"example\": \"light\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-params-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: QueryParams
---
