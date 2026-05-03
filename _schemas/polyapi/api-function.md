---
description: An API function wraps a third-party API call and is invoked through the PolyAPI gateway, providing a managed proxy with built-in authentication, monitoring, and variable injection.
layout: schema
name: PolyAPI API Function
properties_list:
- description: The unique identifier of the API function.
  name: id
  type: string
- description: The name of the API function.
  name: name
  type: string
- description: A description of what the API function does.
  name: description
  type: string
- description: The context path for organizing the function in the catalog.
  name: context
  type: string
- description: The HTTP method used by the API function.
  name: method
  type: string
- description: The target URL for the API call.
  name: url
  type: string
- description: HTTP headers to include in the API call.
  name: headers
  type: object
- description: The request body schema for the API call.
  name: requestBody
  type: object
- description: The expected response schema.
  name: responseSchema
  type: object
- description: The lifecycle state of the function.
  name: state
  type: string
- description: The owner of the function.
  name: owner
  type: string
- description: The visibility of the function.
  name: visibility
  type: string
- description: Timestamp when the function was created.
  name: createdAt
  type: string
- description: Timestamp when the function was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/api-function.json
slug: api-function
source_filename: api-function.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/api-function.json\",\n  \"title\": \"PolyAPI API Function\",\n  \"description\": \"An API function wraps a third-party API call and is invoked through the PolyAPI gateway, providing a managed proxy with built-in authentication, monitoring, and variable injection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the API function.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the API function.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the API function does.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"The context path for organizing the function in the catalog.\"\n    },\n    \"method\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"],\n      \"description\": \"The HTTP method used by the API function.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The target URL for the API call.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"HTTP headers to include in the API call.\"\n    },\n    \"requestBody\": {\n      \"type\": \"object\",\n      \"description\": \"The request body schema for the API call.\"\n    },\n    \"responseSchema\": {\n      \"type\": \"object\",\n      \"description\": \"The expected response schema.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"deprecated\"],\n      \"description\": \"The lifecycle state of the function.\"\n    },\n    \"owner\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The owner of the function.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"The visibility of the function.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the function was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the function was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"method\", \"url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/api-function.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI API Function
---
