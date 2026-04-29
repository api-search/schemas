---
description: LicenseHistoryResponse from Adobe API
layout: schema
name: LicenseHistoryResponse
properties_list:
- description: ''
  name: nb_results
  type: integer
- description: ''
  name: files
  type: array
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-stock-api-license-history-response-schema.json
slug: adobe-stock-api-license-history-response
source_filename: adobe-stock-api-license-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-license-history-response-schema.json\",\n  \"title\": \"LicenseHistoryResponse\",\n  \"description\": \"LicenseHistoryResponse from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          },\n          \"content_type\": {\n            \"type\": \"string\"\n          },\n          \"thumbnail_url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"license\": {\n            \"type\": \"string\"\
  \n          },\n          \"license_date\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"download_url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-license-history-response-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: LicenseHistoryResponse
---
