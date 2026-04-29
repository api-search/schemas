---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: A stable error code describing the type and nature of the error
  name: code
  type: string
- description: A readable description of the error and cause
  name: message
  type: string
- description: Information about what part of the request caused the error
  name: target
  type: string
- description: Additional key/value information about the error
  name: extensionData
  type: object
- description: Nested list of error objects with more details
  name: clientError
  type: array
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-error-response-schema.json
slug: admin-center-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"A stable error code describing the type and nature of the error\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A readable description of the error and cause\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"Information about what part of the request caused the error\"\n    },\n    \"extensionData\": {\n      \"type\": \"object\",\n      \"description\": \"Additional key/value information about the error\"\n    },\n    \"clientError\": {\n      \"type\": \"array\",\n      \"description\": \"Nested list of error objects with more details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-error-response-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ErrorResponse
---
