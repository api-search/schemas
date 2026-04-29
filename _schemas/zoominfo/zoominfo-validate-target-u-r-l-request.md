---
description: ValidateTargetURLRequest schema from ZoomInfo API
layout: schema
name: ValidateTargetURLRequest
properties_list:
- description: ''
  name: targetUrl
  type: string
- description: ''
  name: objectType
  type: string
- description: ''
  name: fullPayload
  type: boolean
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-validate-target-u-r-l-request-schema.json
slug: zoominfo-validate-target-u-r-l-request
source_filename: zoominfo-validate-target-u-r-l-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-validate-target-u-r-l-request-schema.json\",\n  \"title\": \"ValidateTargetURLRequest\",\n  \"description\": \"ValidateTargetURLRequest schema from ZoomInfo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"objectType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"fullPayload\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"targetUrl\",\n    \"objectType\",\n    \"fullPayload\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-validate-target-u-r-l-request-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: ValidateTargetURLRequest
---
