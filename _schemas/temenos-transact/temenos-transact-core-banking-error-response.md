---
description: Standard error response structure
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: header
  type: object
- description: ''
  name: error
  type: object
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-error-response-schema.json
slug: temenos-transact-core-banking-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response structure\",\n  \"properties\": {\n    \"header\": {\n      \"type\": \"object\"\n    },\n    \"error\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-error-response-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: ErrorResponse
---
