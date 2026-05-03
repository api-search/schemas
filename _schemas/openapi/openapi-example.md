---
description: An object representing an example of a schema or parameter.
layout: schema
name: OpenAPI Example Object
properties_list:
- description: Short description for the example.
  name: summary
  type: string
- description: Long description for the example.
  name: description
  type: string
- description: Embedded literal example.
  name: value
  type: object
- description: A URI that points to the literal example.
  name: externalValue
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-example.json
slug: openapi-example
source_filename: openapi-example.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-example.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Example Object\",\n  \"description\": \"An object representing an example of a schema or parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Short description for the example.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Long description for the example.\"\n    },\n    \"value\": {\n      \"description\": \"Embedded literal example.\"\n    },\n    \"externalValue\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URI that points to the literal example.\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-example.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Example Object
---
