---
description: LicenseInfoResponse from Adobe API
layout: schema
name: LicenseInfoResponse
properties_list:
- description: ''
  name: contents
  type: object
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-stock-api-license-info-response-schema.json
slug: adobe-stock-api-license-info-response
source_filename: adobe-stock-api-license-info-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-license-info-response-schema.json\",\n  \"title\": \"LicenseInfoResponse\",\n  \"description\": \"LicenseInfoResponse from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contents\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"content_id\": {\n            \"type\": \"integer\"\n          },\n          \"purchase_details\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"state\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"not_purchased\",\n                  \"purchased\",\n                  \"cancelled\"\n                ]\n              },\n              \"license\": {\n                \"\
  type\": \"string\"\n              },\n              \"date\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"Download URL if already licensed.\"\n              }\n            }\n          },\n          \"size\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-license-info-response-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: LicenseInfoResponse
---
