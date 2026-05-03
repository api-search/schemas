---
description: Schema describing the top-level structure of an OpenAPI 3.1.0 document, the industry standard for defining RESTful APIs.
layout: schema
name: OpenAPI Document
properties_list:
- description: The OpenAPI Specification version. Must be a supported version string.
  name: openapi
  type: string
- description: ''
  name: info
  type: object
- description: The default JSON Schema dialect for Schema Objects in this document.
  name: jsonSchemaDialect
  type: string
- description: An array of Server Objects providing connectivity information to target servers.
  name: servers
  type: array
- description: ''
  name: paths
  type: object
- description: Incoming webhooks that may be received by the API provider.
  name: webhooks
  type: object
- description: ''
  name: components
  type: object
- description: A declaration of which security mechanisms can be used across the API.
  name: security
  type: array
- description: A list of tags used by the document with additional metadata.
  name: tags
  type: array
- description: ''
  name: externalDocs
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-document.json
slug: openapi-document
source_filename: openapi-document.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-document.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Document\",\n  \"description\": \"Schema describing the top-level structure of an OpenAPI 3.1.0 document, the industry standard for defining RESTful APIs.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"openapi\",\n    \"info\"\n  ],\n  \"properties\": {\n    \"openapi\": {\n      \"type\": \"string\",\n      \"description\": \"The OpenAPI Specification version. Must be a supported version string.\",\n      \"pattern\": \"^3\\\\.1\\\\.\\\\d+$\",\n      \"examples\": [\n        \"3.1.0\"\n      ]\n    },\n    \"info\": {\n      \"$ref\": \"openapi-info.json\"\n    },\n    \"jsonSchemaDialect\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The default JSON Schema dialect for Schema Objects in this document.\",\n      \"default\": \"https://spec.openapis.org/oas/3.1/dialect/base\"\n    },\n    \"servers\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"An array of Server Objects providing connectivity information to target servers.\",\n      \"items\": {\n        \"$ref\": \"openapi-server.json\"\n      },\n      \"default\": [\n        {\n          \"url\": \"/\"\n        }\n      ]\n    },\n    \"paths\": {\n      \"$ref\": \"openapi-paths.json\"\n    },\n    \"webhooks\": {\n      \"type\": \"object\",\n      \"description\": \"Incoming webhooks that may be received by the API provider.\",\n      \"additionalProperties\": {\n        \"$ref\": \"openapi-path-item.json\"\n      }\n    },\n    \"components\": {\n      \"$ref\": \"openapi-components.json\"\n    },\n    \"security\": {\n      \"type\": \"array\",\n      \"description\": \"A declaration of which security mechanisms can be used across the API.\",\n      \"items\": {\n        \"$ref\": \"openapi-security-requirement.json\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list\
  \ of tags used by the document with additional metadata.\",\n      \"items\": {\n        \"$ref\": \"openapi-tag.json\"\n      }\n    },\n    \"externalDocs\": {\n      \"$ref\": \"openapi-external-documentation.json\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-document.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Document
---
