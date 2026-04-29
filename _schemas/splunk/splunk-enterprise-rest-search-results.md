---
description: ''
layout: schema
name: SearchResults
properties_list:
- description: Starting offset of results
  name: init_offset
  type: integer
- description: Array of result rows
  name: results
  type: array
- description: Metadata about the fields in the results
  name: fields
  type: array
- description: ''
  name: messages
  type: array
- description: Whether results are preview (partial) results
  name: preview
  type: boolean
- description: Highlighted terms in results
  name: highlighted
  type: object
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-search-results-schema.json
slug: splunk-enterprise-rest-search-results
source_filename: splunk-enterprise-rest-search-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResults\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"init_offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting offset of results\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of result rows\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"Metadata about the fields in the results\"\n    },\n    \"messages\": {\n      \"type\": \"array\"\n    },\n    \"preview\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether results are preview (partial) results\"\n    },\n    \"highlighted\": {\n      \"type\": \"object\",\n      \"description\": \"Highlighted terms in results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-search-results-schema.json
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
title: SearchResults
---
