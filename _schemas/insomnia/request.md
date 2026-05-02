---
description: An Insomnia request represents an individual HTTP, GraphQL, gRPC, WebSocket, or other protocol request configured within a workspace. It contains the URL, method, headers, body, authentication, and other settings needed to execute the request.
layout: schema
name: Insomnia Request
properties_list:
- description: Unique identifier for the request, typically prefixed with req_.
  name: _id
  type: string
- description: Human-readable name of the request.
  name: name
  type: string
- description: Optional description providing context about the request.
  name: description
  type: string
- description: The target URL for the request, which may include Insomnia template tags.
  name: url
  type: string
- description: HTTP method for the request.
  name: method
  type: string
- description: List of HTTP headers to include in the request.
  name: headers
  type: array
- description: Query parameters appended to the request URL.
  name: parameters
  type: array
- description: The request body configuration.
  name: body
  type: object
- description: Authentication configuration for the request.
  name: authentication
  type: object
- description: Identifier of the parent workspace or folder.
  name: parentId
  type: string
- description: Whether to follow HTTP redirects.
  name: settingFollowRedirects
  type: string
- description: Whether to send cookies with the request.
  name: settingSendCookies
  type: boolean
- description: Whether to store cookies from the response.
  name: settingStoreCookies
  type: boolean
- description: Whether to encode the request path automatically.
  name: settingRebuildPath
  type: boolean
- description: Unix timestamp in milliseconds when the request was created.
  name: created
  type: integer
- description: Unix timestamp in milliseconds when the request was last modified.
  name: modified
  type: integer
- description: The resource type identifier.
  name: _type
  type: string
provider_name: Insomnia
provider_slug: insomnia
schema_file: json-schema/request.json
slug: request
source_filename: request.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/json-schema/request.json\",\n  \"title\": \"Insomnia Request\",\n  \"description\": \"An Insomnia request represents an individual HTTP, GraphQL, gRPC, WebSocket, or other protocol request configured within a workspace. It contains the URL, method, headers, body, authentication, and other settings needed to execute the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the request, typically prefixed with req_.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the request.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description providing context about the request.\"\n    },\n    \"url\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The target URL for the request, which may include Insomnia template tags.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\", \"TRACE\"],\n      \"description\": \"HTTP method for the request.\"\n    },\n    \"headers\": {\n      \"type\": \"array\",\n      \"description\": \"List of HTTP headers to include in the request.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Header name.\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Header value.\"\n          },\n          \"disabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this header is disabled.\",\n            \"default\": false\n          }\n        },\n        \"required\": [\"name\", \"value\"\
  ]\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Query parameters appended to the request URL.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Parameter name.\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Parameter value.\"\n          },\n          \"disabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this parameter is disabled.\",\n            \"default\": false\n          }\n        },\n        \"required\": [\"name\", \"value\"]\n      }\n    },\n    \"body\": {\n      \"type\": \"object\",\n      \"description\": \"The request body configuration.\",\n      \"properties\": {\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the request body (e.g., application/json, multipart/form-data).\"\
  \n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Raw text content of the request body.\"\n        },\n        \"params\": {\n          \"type\": \"array\",\n          \"description\": \"Form data parameters when using form-encoded or multipart body types.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              },\n              \"disabled\": {\n                \"type\": \"boolean\",\n                \"default\": false\n              }\n            },\n            \"required\": [\"name\", \"value\"]\n          }\n        }\n      }\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration for the request.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Authentication type (e.g., bearer, basic, oauth2, apikey).\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Token value for bearer authentication.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Username for basic authentication.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Password for basic authentication.\"\n        },\n        \"disabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether authentication is disabled for this request.\",\n          \"default\": false\n        }\n      }\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent workspace or folder.\"\n    },\n    \"settingFollowRedirects\": {\n      \"type\": \"string\",\n      \"enum\": [\"on\", \"off\", \"global\"],\n      \"description\": \"Whether to\
  \ follow HTTP redirects.\",\n      \"default\": \"global\"\n    },\n    \"settingSendCookies\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send cookies with the request.\",\n      \"default\": true\n    },\n    \"settingStoreCookies\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to store cookies from the response.\",\n      \"default\": true\n    },\n    \"settingRebuildPath\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to encode the request path automatically.\",\n      \"default\": true\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the request was created.\"\n    },\n    \"modified\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the request was last modified.\"\n    },\n    \"_type\": {\n      \"type\": \"string\",\n      \"const\": \"request\",\n      \"description\": \"The resource type identifier.\"\
  \n    }\n  },\n  \"required\": [\"_id\", \"name\", \"url\", \"method\", \"parentId\", \"_type\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/json-schema/request.json
tags:
- API Design
- CLI
- Clients
- Mocking
- Platform
- Testing
title: Insomnia Request
---
