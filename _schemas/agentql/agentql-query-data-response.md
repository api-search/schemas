---
description: Response containing extracted structured data.
layout: schema
name: QueryDataResponse
properties_list:
- description: Extracted data matching the structure defined in the query.
  name: data
  type: object
- description: ''
  name: metadata
  type: object
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-query-data-response-schema.json
slug: agentql-query-data-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-data-response-schema.json\",\n  \"title\": \"QueryDataResponse\",\n  \"description\": \"Response containing extracted structured data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Extracted data matching the structure defined in the query.\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/ResponseMetadata\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-data-response-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: QueryDataResponse
---
