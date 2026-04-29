---
description: API response containing a list of exported services.
layout: schema
name: ServiceListResponse
properties_list:
- description: HTTP status code.
  name: statusCode
  type: integer
- description: Human-readable status description.
  name: statusDescription
  type: string
- description: Success message.
  name: successMessage
  type: string
- description: Array of exported service entries.
  name: data
  type: array
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-service-list-response-schema.json
slug: apache-ofbiz-service-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-list-response-schema.json\",\n  \"title\": \"ServiceListResponse\",\n  \"description\": \"API response containing a list of exported services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 200\n    },\n    \"statusDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status description.\",\n      \"example\": \"OK\"\n    },\n    \"successMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Success message.\",\n      \"example\": \"OK\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of exported service entries.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\"\
  : \"A single exported OFBiz service with its metadata and invocation link.\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The service name.\",\n            \"example\": \"findProductById\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable description of the service.\",\n            \"example\": \"Finds productId(s) corresponding to a product reference.\"\n          },\n          \"link\": {\n            \"type\": \"object\",\n            \"description\": \"Hypermedia link to a service endpoint.\",\n            \"properties\": {\n              \"href\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"URL to invoke the service.\",\n                \"example\": \"https://localhost:8443/rest/services/findProductById\"\n              },\n              \"rel\": {\n              \
  \  \"type\": \"string\",\n                \"description\": \"Relationship type.\",\n                \"example\": \"self\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"HTTP method for accessing the service.\",\n                \"example\": \"get\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-list-response-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: ServiceListResponse
---
