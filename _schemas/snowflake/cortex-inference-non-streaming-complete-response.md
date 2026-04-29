---
description: Text-completion response for non-streaming request.
layout: schema
name: NonStreamingCompleteResponse
properties_list:
- description: ''
  name: choices
  type: array
- description: ''
  name: usage
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-inference-non-streaming-complete-response-schema.json
slug: cortex-inference-non-streaming-complete-response
source_filename: cortex-inference-non-streaming-complete-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NonStreamingCompleteResponse\",\n  \"type\": \"object\",\n  \"description\": \"Text-completion response for non-streaming request.\",\n  \"properties\": {\n    \"choices\": {\n      \"type\": \"array\"\n    },\n    \"usage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-inference-non-streaming-complete-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NonStreamingCompleteResponse
---
