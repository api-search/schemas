---
description: A schema representing the key properties and constraints of a RESTful API following the Representational State Transfer architectural style.
layout: schema
name: REST API
properties_list:
- description: The name of the REST API.
  name: name
  type: string
- description: A description of the API's purpose and capabilities.
  name: description
  type: string
- description: The version of the API.
  name: version
  type: string
- description: The base URL of the API server.
  name: baseUrl
  type: string
- description: The resources exposed by the API.
  name: resources
  type: array
- description: Authentication scheme used by the API.
  name: authentication
  type: object
- description: Content formats supported by the API.
  name: formats
  type: array
provider_name: REST
provider_slug: rest
schema_file: json-schema/rest-api-schema.json
slug: rest-api
source_filename: rest-api-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/rest/json-schema/rest-api-schema.json\",\n  \"title\": \"REST API\",\n  \"description\": \"A schema representing the key properties and constraints of a RESTful API following the Representational State Transfer architectural style.\",\n  \"type\": \"object\",\n  \"required\": [\"baseUrl\", \"resources\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the REST API.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the API's purpose and capabilities.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the API.\",\n      \"examples\": [\"1.0.0\", \"2.1.0\", \"v3\"]\n    },\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The base URL of the API server.\"\
  \n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"The resources exposed by the API.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Resource\"\n      }\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication scheme used by the API.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"apikey\", \"bearer\", \"basic\", \"oauth2\"],\n          \"description\": \"The authentication mechanism.\"\n        }\n      }\n    },\n    \"formats\": {\n      \"type\": \"array\",\n      \"description\": \"Content formats supported by the API.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"examples\": [\"application/json\", \"application/xml\", \"text/html\"]\n      }\n    }\n  },\n  \"$defs\": {\n    \"Resource\": {\n      \"type\": \"object\",\n      \"required\": [\"path\"],\n      \"description\": \"A named information resource identified\
  \ by a URI path.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name.\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"The URI path pattern (may include {parameter} templates).\"\n        },\n        \"methods\": {\n          \"type\": \"array\",\n          \"description\": \"HTTP methods supported by this resource.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\"]\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rest/refs/heads/main/json-schema/rest-api-schema.json
tags:
- API Design
- Architecture
- HTTP
- REST
- RESTful
- Web Services
title: REST API
---
