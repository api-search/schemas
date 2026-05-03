---
description: Represents an HTTP request in RestSharp. Defines the resource path, HTTP method, parameters, body, and per-request options.
layout: schema
name: RestRequest
properties_list:
- description: Resource path relative to the client's base URL (e.g., /users/{id})
  name: resource
  type: string
- description: 'HTTP method for the request. Default: GET'
  name: method
  type: string
- description: List of parameters (path, query, header, cookie, form, body)
  name: parameters
  type: array
- description: Request-level timeout override in milliseconds
  name: timeout
  type: integer
- description: Format for the request body serialization
  name: requestFormat
  type: string
- description: Files to include in a multipart form request
  name: files
  type: array
provider_name: RestSharp
provider_slug: restsharp
schema_file: json-schema/restsharp-rest-request-schema.json
slug: restsharp-rest-request
source_filename: restsharp-rest-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://restsharp.dev/schemas/rest-request\",\n  \"title\": \"RestRequest\",\n  \"description\": \"Represents an HTTP request in RestSharp. Defines the resource path, HTTP method, parameters, body, and per-request options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"Resource path relative to the client's base URL (e.g., /users/{id})\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\", \"HEAD\", \"OPTIONS\"],\n      \"description\": \"HTTP method for the request. Default: GET\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"List of parameters (path, query, header, cookie, form, body)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Parameter\"\n      }\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Request-level timeout override in milliseconds\"\n    },\n    \"requestFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\"Json\", \"Xml\", \"MultipartFormData\", \"UrlEncodedForm\"],\n      \"description\": \"Format for the request body serialization\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"Files to include in a multipart form request\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"fileName\": { \"type\": \"string\" },\n          \"contentType\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Parameter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Parameter name\"\n        },\n        \"value\": {\n          \"description\": \"Parameter value\"\n        },\n        \"type\": {\n         \
  \ \"type\": \"string\",\n          \"enum\": [\"UrlSegment\", \"QueryString\", \"HttpHeader\", \"RequestBody\", \"Cookie\", \"GetOrPost\"],\n          \"description\": \"Where the parameter is placed in the request\"\n        },\n        \"contentType\": {\n          \"type\": \"string\",\n          \"description\": \"Content-Type for body parameters\"\n        },\n        \"encode\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to URL-encode the parameter value\"\n        }\n      },\n      \"required\": [\"name\", \"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restsharp/refs/heads/main/json-schema/restsharp-rest-request-schema.json
tags:
- .NET
- Apache License
- C#
- HTTP Client
- NuGet
- Open Source
- SDKs
title: RestRequest
---
