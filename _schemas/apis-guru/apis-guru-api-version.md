---
description: ApiVersion schema from APIs.guru REST API
layout: schema
name: ApiVersion
properties_list:
- description: Timestamp when the version was added
  name: added
  type: string
- description: Copy of `externalDocs` section from OpenAPI definition
  name: externalDocs
  type: object
- description: Copy of `info` section from OpenAPI definition
  name: info
  type: object
- description: Link to the individual API entry for this API
  name: link
  type: string
- description: The value of the `openapi` or `swagger` property of the source definition
  name: openapiVer
  type: string
- description: URL to OpenAPI definition in JSON format
  name: swaggerUrl
  type: string
- description: URL to OpenAPI definition in YAML format
  name: swaggerYamlUrl
  type: string
- description: Timestamp when the version was updated
  name: updated
  type: string
provider_name: APIs.guru
provider_slug: apis-guru
schema_file: json-schema/apis-guru-api-version-schema.json
slug: apis-guru-api-version
source_filename: apis-guru-api-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-api-version-schema.json\",\n  \"title\": \"ApiVersion\",\n  \"description\": \"ApiVersion schema from APIs.guru REST API\",\n  \"additionalProperties\": false,\n  \"properties\": {\n    \"added\": {\n      \"description\": \"Timestamp when the version was added\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"externalDocs\": {\n      \"description\": \"Copy of `externalDocs` section from OpenAPI definition\",\n      \"minProperties\": 1,\n      \"type\": \"object\"\n    },\n    \"info\": {\n      \"description\": \"Copy of `info` section from OpenAPI definition\",\n      \"minProperties\": 1,\n      \"type\": \"object\"\n    },\n    \"link\": {\n      \"description\": \"Link to the individual API entry for this API\",\n      \"format\": \"url\",\n      \"type\": \"string\"\
  \n    },\n    \"openapiVer\": {\n      \"description\": \"The value of the `openapi` or `swagger` property of the source definition\",\n      \"type\": \"string\"\n    },\n    \"swaggerUrl\": {\n      \"description\": \"URL to OpenAPI definition in JSON format\",\n      \"format\": \"url\",\n      \"type\": \"string\"\n    },\n    \"swaggerYamlUrl\": {\n      \"description\": \"URL to OpenAPI definition in YAML format\",\n      \"format\": \"url\",\n      \"type\": \"string\"\n    },\n    \"updated\": {\n      \"description\": \"Timestamp when the version was updated\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"added\",\n    \"updated\",\n    \"swaggerUrl\",\n    \"swaggerYamlUrl\",\n    \"info\",\n    \"openapiVer\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-api-version-schema.json
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
title: ApiVersion
---
