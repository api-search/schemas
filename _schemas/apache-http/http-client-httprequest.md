---
description: HTTP request configuration for Apache HttpComponents client
layout: schema
name: HttpRequest
properties_list:
- description: HTTP method
  name: method
  type: string
- description: Request URI
  name: uri
  type: string
- description: Request headers as key-value pairs
  name: headers
  type: object
- description: Request body content
  name: body
  type: string
- description: Content-Type header value
  name: contentType
  type: string
provider_name: Apache HttpComponents
provider_slug: apache-http
schema_file: json-schema/http-client-httprequest-schema.json
slug: http-client-httprequest
source_filename: http-client-httprequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-http/json-schema/http-client-httprequest-schema.json\",\n  \"title\": \"HttpRequest\",\n  \"type\": \"object\",\n  \"description\": \"HTTP request configuration for Apache HttpComponents client\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method\",\n      \"example\": \"GET\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Request URI\",\n      \"example\": \"https://api.example.com/data\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Request headers as key-value pairs\",\n      \"example\": {\n        \"Accept\": \"application/json\",\n        \"Authorization\": \"Bearer token\"\n      }\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Request body content\",\n      \"example\": \"{\\\"key\\\": \\\"value\\\
  \"}\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Content-Type header value\",\n      \"example\": \"application/json\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-http/refs/heads/main/json-schema/http-client-httprequest-schema.json
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: HttpRequest
---
