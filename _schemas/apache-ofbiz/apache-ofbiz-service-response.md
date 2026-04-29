---
description: Standard API response from an OFBiz service invocation.
layout: schema
name: ServiceResponse
properties_list:
- description: HTTP status code.
  name: statusCode
  type: integer
- description: Human-readable status description.
  name: statusDescription
  type: string
- description: Success message if applicable.
  name: successMessage
  type: string
- description: Service output data. Structure varies by service.
  name: data
  type: object
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-service-response-schema.json
slug: apache-ofbiz-service-response
source_filename: apache-ofbiz-service-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-response-schema.json\",\n  \"title\": \"ServiceResponse\",\n  \"description\": \"Standard API response from an OFBiz service invocation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 200\n    },\n    \"statusDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status description.\",\n      \"example\": \"OK\"\n    },\n    \"successMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Success message if applicable.\",\n      \"example\": \"OK\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Service output data. Structure varies by service.\"\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-response-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: ServiceResponse
---
