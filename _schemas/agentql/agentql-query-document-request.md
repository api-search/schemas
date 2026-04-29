---
description: Request body for querying data from a document.
layout: schema
name: QueryDocumentRequest
properties_list:
- description: URL of the document to query (PDF or image).
  name: url
  type: string
- description: AgentQL query string for structured data extraction.
  name: query
  type: string
- description: Natural language description of the data to extract.
  name: prompt
  type: string
provider_name: AgentQL
provider_slug: agentql
schema_file: json-schema/agentql-query-document-request-schema.json
slug: agentql-query-document-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-document-request-schema.json\",\n  \"title\": \"QueryDocumentRequest\",\n  \"description\": \"Request body for querying data from a document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the document to query (PDF or image).\",\n      \"example\": \"https://example.com/invoice.pdf\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"AgentQL query string for structured data extraction.\",\n      \"example\": \"{ invoice { total_amount vendor_name date } }\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language description of the data to extract.\",\n      \"example\": \"Extract invoice totals and vendor information\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/json-schema/agentql-query-document-request-schema.json
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
title: QueryDocumentRequest
---
