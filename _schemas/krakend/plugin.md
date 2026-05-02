---
description: Plugin loader configuration for KrakenD, defining the directory and patterns for loading external Go plugins at gateway startup.
layout: schema
name: KrakenD Plugin Configuration
properties_list:
- description: File pattern to match plugin shared object files. E.g., .so.
  name: pattern
  type: string
- description: Directory path where plugin .so files are located.
  name: folder
  type: string
provider_name: KrakenD
provider_slug: krakend
schema_file: json-schema/plugin.json
slug: plugin
source_filename: plugin.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/krakend/blob/main/json-schema/plugin.json\",\n  \"title\": \"KrakenD Plugin Configuration\",\n  \"description\": \"Plugin loader configuration for KrakenD, defining the directory and patterns for loading external Go plugins at gateway startup.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"File pattern to match plugin shared object files. E.g., .so.\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"description\": \"Directory path where plugin .so files are located.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/json-schema/plugin.json
tags:
- Aggregation
- API Gateway
- Go
- Open Source
title: KrakenD Plugin Configuration
---
