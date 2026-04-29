---
description: Request body for querying data from a web page.
layout: schema
name: QueryDataRequest
properties_list:
- description: The URL of the web page to query.
  name: url
  type: string
- description: Raw HTML content to query instead of a URL.
  name: html
  type: string
- description: AgentQL query string for structured data extraction.
  name: query
  type: string
- description: Natural language description of the data to extract (alternative to query).
  name: prompt
  type: string
- description: ''
  name: params
  type: object
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-query-data-request-schema.json
slug: agentql-query-data-request
source_filename: agentql-query-data-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-data-request-schema.json\",\n  \"title\": \"QueryDataRequest\",\n  \"description\": \"Request body for querying data from a web page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the web page to query.\",\n      \"example\": \"https://news.ycombinator.com\"\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"Raw HTML content to query instead of a URL.\",\n      \"example\": \"<html><body><h1>Hello World</h1></body></html>\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"AgentQL query string for structured data extraction.\",\n      \"example\": \"{ posts[] { title link score } }\"\n    },\n    \"prompt\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Natural language description of the data to extract (alternative to query).\",\n      \"example\": \"Extract the top 10 posts with their titles, links, and scores\"\n    },\n    \"params\": {\n      \"$ref\": \"#/components/schemas/QueryParams\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-data-request-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: QueryDataRequest
---
