---
description: Current status and result of a PDF Services operation
layout: schema
name: OperationStatus
properties_list:
- description: Current status of the operation
  name: status
  type: string
- description: ''
  name: asset
  type: object
- description: Error details if the operation failed
  name: errors
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-operation-status-schema.json
slug: adobe-creative-suite-pdf-services-operation-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-operation-status-schema.json\",\n  \"title\": \"OperationStatus\",\n  \"description\": \"Current status and result of a PDF Services operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the operation\",\n      \"enum\": [\n        \"in progress\",\n        \"done\",\n        \"failed\"\n      ],\n      \"example\": \"done\"\n    },\n    \"asset\": {\n      \"$ref\": \"#/components/schemas/Asset\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Error details if the operation failed\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": {\n            \"type\": \"string\"\n          },\n   \
  \       \"message\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-operation-status-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: OperationStatus
---
