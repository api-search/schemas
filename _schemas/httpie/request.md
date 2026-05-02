---
description: Schema representing an HTTPie HTTP request, including method, URL, headers, and body.
layout: schema
name: HTTPie Request
properties_list:
- description: The HTTP method for the request.
  name: method
  type: string
- description: The target URL for the request.
  name: url
  type: string
- description: HTTP headers to include in the request.
  name: headers
  type: object
- description: Query string parameters appended to the URL.
  name: queryParams
  type: object
- description: The request body payload.
  name: body
  type: object
- description: Authentication credentials for the request.
  name: auth
  type: object
- description: Request timeout in seconds.
  name: timeout
  type: number
- description: Whether to verify SSL certificates.
  name: verify
  type: boolean
provider_name: HTTPie
provider_slug: httpie
schema_file: json-schema/request.json
slug: request
source_filename: request.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/json-schema/request.json\",\n  \"title\": \"HTTPie Request\",\n  \"description\": \"Schema representing an HTTPie HTTP request, including method, URL, headers, and body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP method for the request.\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\"]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The target URL for the request.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP headers to include in the request.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"queryParams\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Query string parameters appended to the URL.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"body\": {\n      \"description\": \"The request body payload.\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"object\" }\n      ]\n    },\n    \"auth\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication credentials for the request.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The authentication type.\",\n          \"enum\": [\"basic\", \"bearer\", \"digest\"]\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Username for basic or digest authentication.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Password for basic or digest authentication.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Token for bearer authentication.\"\n        }\n      },\n      \"required\": [\"type\"]\n    },\n    \"timeout\": {\n      \"type\": \"number\",\n      \"description\": \"Request timeout in seconds.\"\n    },\n    \"verify\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to verify SSL certificates.\",\n      \"default\": true\n    }\n  },\n  \"required\": [\"method\", \"url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/json-schema/request.json
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
title: HTTPie Request
---
