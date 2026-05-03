---
description: Configuration options for the RestSharp RestClient. Passed to the RestClient constructor to configure base URL, authentication, timeouts, redirects, and HTTP client behavior.
layout: schema
name: RestClientOptions
properties_list:
- description: Base URL for all requests made by this client
  name: baseUrl
  type: string
- description: IAuthenticator implementation for request authentication (OAuth1, OAuth2, HTTP Basic, JWT Bearer)
  name: authenticator
  type: object
- description: Request timeout in milliseconds. 0 = no timeout (use with caution)
  name: timeout
  type: integer
- description: Maximum request timeout in milliseconds
  name: maxTimeout
  type: integer
- description: 'Whether to automatically follow HTTP redirects. Default: true'
  name: followRedirects
  type: boolean
- description: Maximum number of redirects to follow
  name: maxRedirects
  type: integer
- description: 'User-Agent header value. Default: RestSharp/{version}'
  name: userAgent
  type: string
- description: Default encoding for request and response content
  name: encoding
  type: string
- description: 'Whether to send credentials with the first request. Default: false'
  name: preAuthenticate
  type: boolean
- description: 'Whether to use default system credentials. Default: false'
  name: useDefaultCredentials
  type: boolean
- description: 'Whether to omit charset from Content-Type header. Default: false'
  name: disableCharset
  type: boolean
- description: 'Whether to allow multiple default parameters with the same name. Default: false'
  name: allowMultipleDefaultParametersWithSameName
  type: boolean
provider_name: RestSharp
provider_slug: restsharp
schema_file: json-schema/restsharp-rest-client-options-schema.json
slug: restsharp-rest-client-options
source_filename: restsharp-rest-client-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://restsharp.dev/schemas/rest-client-options\",\n  \"title\": \"RestClientOptions\",\n  \"description\": \"Configuration options for the RestSharp RestClient. Passed to the RestClient constructor to configure base URL, authentication, timeouts, redirects, and HTTP client behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL for all requests made by this client\"\n    },\n    \"authenticator\": {\n      \"type\": \"object\",\n      \"description\": \"IAuthenticator implementation for request authentication (OAuth1, OAuth2, HTTP Basic, JWT Bearer)\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Request timeout in milliseconds. 0 = no timeout (use with caution)\"\n    },\n    \"maxTimeout\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Maximum request timeout in milliseconds\"\n    },\n    \"followRedirects\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically follow HTTP redirects. Default: true\",\n      \"default\": true\n    },\n    \"maxRedirects\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of redirects to follow\"\n    },\n    \"userAgent\": {\n      \"type\": \"string\",\n      \"description\": \"User-Agent header value. Default: RestSharp/{version}\"\n    },\n    \"encoding\": {\n      \"type\": \"string\",\n      \"description\": \"Default encoding for request and response content\"\n    },\n    \"preAuthenticate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send credentials with the first request. Default: false\",\n      \"default\": false\n    },\n    \"useDefaultCredentials\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use default system credentials. Default: false\",\n      \"default\"\
  : false\n    },\n    \"disableCharset\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to omit charset from Content-Type header. Default: false\",\n      \"default\": false\n    },\n    \"allowMultipleDefaultParametersWithSameName\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow multiple default parameters with the same name. Default: false\",\n      \"default\": false\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restsharp/refs/heads/main/json-schema/restsharp-rest-client-options-schema.json
tags:
- .NET
- Apache License
- C#
- HTTP Client
- NuGet
- Open Source
- SDKs
title: RestClientOptions
---
