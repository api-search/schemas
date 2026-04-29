---
description: A document or data conversion request to the ApyHub API
layout: schema
name: ConversionRequest
properties_list:
- description: Unique conversion request identifier
  name: requestId
  type: string
- description: Conversion operation type
  name: type
  type: string
- description: URL of the input file to convert
  name: inputUrl
  type: string
- description: Desired output format
  name: outputFormat
  type: string
- description: Conversion status
  name: status
  type: string
- description: URL of the converted output file
  name: outputUrl
  type: string
- description: Request creation timestamp
  name: createdAt
  type: string
provider_name: ApyHub
provider_slug: apyhub
schema_file: json-schema/conversion-request-schema.json
slug: conversion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apyhub/main/json-schema/conversion-request-schema.json\",\n  \"title\": \"ConversionRequest\",\n  \"description\": \"A document or data conversion request to the ApyHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique conversion request identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pdf\",\n        \"html-to-pdf\",\n        \"word-to-pdf\",\n        \"image-resize\",\n        \"currency\",\n        \"extract-text\"\n      ],\n      \"description\": \"Conversion operation type\"\n    },\n    \"inputUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the input file to convert\"\n    },\n    \"outputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Desired output format\"\n   \
  \ },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Conversion status\"\n    },\n    \"outputUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the converted output file\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Request creation timestamp\"\n    }\n  },\n  \"required\": [\n    \"requestId\",\n    \"type\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apyhub/refs/heads/main/json-schema/conversion-request-schema.json
tags:
- API Platform
- Data Processing
- Document Conversion
- Utility APIs
title: ConversionRequest
---
