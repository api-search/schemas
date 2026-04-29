---
description: HTTP response from Apache HttpComponents client execution
layout: schema
name: HttpResponse
properties_list:
- description: HTTP response status code
  name: statusCode
  type: integer
- description: HTTP reason phrase
  name: reasonPhrase
  type: string
- description: Response headers as key-value pairs
  name: headers
  type: object
- description: Response body content
  name: body
  type: string
- description: Content-Type of the response body
  name: contentType
  type: string
provider_name: Apache HttpComponents
provider_slug: apache-http
schema_file: json-schema/http-client-httpresponse-schema.json
slug: http-client-httpresponse
source_filename: http-client-httpresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-http/json-schema/http-client-httpresponse-schema.json\",\n  \"title\": \"HttpResponse\",\n  \"type\": \"object\",\n  \"description\": \"HTTP response from Apache HttpComponents client execution\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP response status code\",\n      \"example\": 200\n    },\n    \"reasonPhrase\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP reason phrase\",\n      \"example\": \"OK\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Response headers as key-value pairs\",\n      \"example\": {\n        \"Content-Type\": \"application/json\"\n      }\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Response body content\",\n      \"example\": \"{\\\"result\\\": \\\"ok\\\"}\"\n    },\n    \"contentType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Content-Type of the response body\",\n      \"example\": \"application/json\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-http/refs/heads/main/json-schema/http-client-httpresponse-schema.json
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: HttpResponse
---
