---
description: Schema for a REST Assured HTTP request specification, representing the given() clause of a REST Assured test.
layout: schema
name: REST Assured Request Specification
properties_list:
- description: The base URI for the API under test.
  name: baseUri
  type: string
- description: The base path appended to the base URI.
  name: basePath
  type: string
- description: The port number for the API under test.
  name: port
  type: integer
- description: HTTP headers to include in the request.
  name: headers
  type: object
- description: Query parameters to append to the request URL.
  name: queryParameters
  type: object
- description: Path parameter values for URI templates.
  name: pathParameters
  type: object
- description: The request body payload.
  name: body
  type: object
- description: The Content-Type header value for the request body.
  name: contentType
  type: string
- description: The Accept header value specifying the desired response format.
  name: accept
  type: string
- description: ''
  name: authentication
  type: object
- description: Cookies to send with the request.
  name: cookies
  type: object
- description: Connection timeout in milliseconds.
  name: timeout
  type: integer
provider_name: REST Assured
provider_slug: rest-assured
schema_file: json-schema/rest-assured-request-schema.json
slug: rest-assured-request
source_filename: rest-assured-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rest-assured.io/schemas/request\",\n  \"title\": \"REST Assured Request Specification\",\n  \"description\": \"Schema for a REST Assured HTTP request specification, representing the given() clause of a REST Assured test.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The base URI for the API under test.\"\n    },\n    \"basePath\": {\n      \"type\": \"string\",\n      \"description\": \"The base path appended to the base URI.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"description\": \"The port number for the API under test.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"HTTP headers to include in the\
  \ request.\"\n    },\n    \"queryParameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          { \"type\": \"string\" },\n          { \"type\": \"number\" },\n          { \"type\": \"boolean\" }\n        ]\n      },\n      \"description\": \"Query parameters to append to the request URL.\"\n    },\n    \"pathParameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Path parameter values for URI templates.\"\n    },\n    \"body\": {\n      \"description\": \"The request body payload.\",\n      \"oneOf\": [\n        { \"type\": \"object\" },\n        { \"type\": \"array\" },\n        { \"type\": \"string\" }\n      ]\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The Content-Type header value for the request body.\",\n      \"examples\": [\"application/json\", \"application/xml\", \"multipart/form-data\"]\n    },\n\
  \    \"accept\": {\n      \"type\": \"string\",\n      \"description\": \"The Accept header value specifying the desired response format.\",\n      \"examples\": [\"application/json\", \"application/xml\"]\n    },\n    \"authentication\": {\n      \"$ref\": \"#/$defs/Authentication\"\n    },\n    \"cookies\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Cookies to send with the request.\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Connection timeout in milliseconds.\"\n    }\n  },\n  \"$defs\": {\n    \"Authentication\": {\n      \"title\": \"Authentication\",\n      \"description\": \"Authentication configuration for the request.\",\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"basic\", \"digest\", \"oauth2\", \"preemptive\"\
  , \"certificate\"],\n          \"description\": \"The authentication scheme to use.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Username for basic or digest authentication.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Password for basic or digest authentication.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Bearer token for OAuth2 authentication.\"\n        },\n        \"keystorePath\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the keystore file for certificate authentication.\"\n        },\n        \"keystorePassword\": {\n          \"type\": \"string\",\n          \"description\": \"Password for the keystore file.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rest-assured/refs/heads/main/json-schema/rest-assured-request-schema.json
tags:
- Functional Testing
- Testing
- Java
- API Testing
- Automation
title: REST Assured Request Specification
---
