---
description: Schema representing an HTTPie HTTP response, including status, headers, and body.
layout: schema
name: HTTPie Response
properties_list:
- description: The HTTP status code of the response.
  name: statusCode
  type: integer
- description: The HTTP status text accompanying the status code.
  name: statusText
  type: string
- description: The HTTP version used in the response.
  name: httpVersion
  type: string
- description: HTTP response headers.
  name: headers
  type: object
- description: The response body content.
  name: body
  type: object
- description: The MIME type of the response body.
  name: contentType
  type: string
- description: Time elapsed for the request-response cycle in seconds.
  name: elapsed
  type: number
- description: The character encoding of the response body.
  name: encoding
  type: string
provider_name: HTTPie
provider_slug: httpie
schema_file: json-schema/response.json
slug: response
source_filename: response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/json-schema/response.json\",\n  \"title\": \"HTTPie Response\",\n  \"description\": \"Schema representing an HTTPie HTTP response, including status, headers, and body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the response.\",\n      \"minimum\": 100,\n      \"maximum\": 599\n    },\n    \"statusText\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP status text accompanying the status code.\"\n    },\n    \"httpVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP version used in the response.\",\n      \"examples\": [\"HTTP/1.1\", \"HTTP/2\"]\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP response headers.\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"body\": {\n      \"description\": \"The response body content.\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"object\" }\n      ]\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the response body.\"\n    },\n    \"elapsed\": {\n      \"type\": \"number\",\n      \"description\": \"Time elapsed for the request-response cycle in seconds.\"\n    },\n    \"encoding\": {\n      \"type\": \"string\",\n      \"description\": \"The character encoding of the response body.\",\n      \"examples\": [\"utf-8\", \"ascii\", \"iso-8859-1\"]\n    }\n  },\n  \"required\": [\"statusCode\", \"headers\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/json-schema/response.json
tags:
- API Client
- API Testing
- CLI
- Client
- Command Line
- Developer Tools
- HTTP
- Open Source
- Sessions
title: HTTPie Response
---
