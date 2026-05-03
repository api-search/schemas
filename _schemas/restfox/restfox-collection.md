---
description: Represents a Restfox API collection containing organized HTTP requests, environment variables, and test configurations for API testing.
layout: schema
name: Restfox Collection
properties_list:
- description: Unique identifier for the collection.
  name: id
  type: string
- description: Human-readable name for the collection.
  name: name
  type: string
- description: Optional description of the collection's purpose.
  name: description
  type: string
- description: List of HTTP requests in the collection.
  name: requests
  type: array
- description: Environment configurations for variable substitution.
  name: environments
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Restfox
provider_slug: restfox
schema_file: json-schema/restfox-collection-schema.json
slug: restfox-collection
source_filename: restfox-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/restfox/refs/heads/main/json-schema/restfox-collection-schema.json\",\n  \"title\": \"Restfox Collection\",\n  \"description\": \"Represents a Restfox API collection containing organized HTTP requests, environment variables, and test configurations for API testing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the collection.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the collection.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the collection's purpose.\"\n    },\n    \"requests\": {\n      \"type\": \"array\",\n      \"description\": \"List of HTTP requests in the collection.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Request\"\
  \n      }\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"Environment configurations for variable substitution.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Environment\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"Request\": {\n      \"type\": \"object\",\n      \"description\": \"An individual HTTP request in a Restfox collection.\",\n      \"properties\": {\n        \"id\": {\"type\": \"string\"},\n        \"name\": {\"type\": \"string\", \"description\": \"Request name displayed in the UI.\"},\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method.\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"HEAD\", \"OPTIONS\", \"TRACE\"]\n        },\n        \"url\"\
  : {\"type\": \"string\", \"description\": \"Request URL, may include environment variable placeholders.\"},\n        \"headers\": {\n          \"type\": \"array\",\n          \"items\": {\"$ref\": \"#/$defs/Header\"}\n        },\n        \"body\": {\n          \"type\": \"object\",\n          \"description\": \"Request body configuration.\",\n          \"properties\": {\n            \"contentType\": {\"type\": \"string\"},\n            \"body\": {\"type\": \"string\"}\n          }\n        },\n        \"description\": {\"type\": \"string\"},\n        \"parentId\": {\"type\": [\"string\", \"null\"], \"description\": \"Parent folder ID for nested organization.\"}\n      },\n      \"required\": [\"method\", \"url\"]\n    },\n    \"Header\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\"type\": \"string\"},\n        \"value\": {\"type\": \"string\"},\n        \"enabled\": {\"type\": \"boolean\", \"default\": true}\n      },\n      \"required\": [\"name\", \"\
  value\"]\n    },\n    \"Environment\": {\n      \"type\": \"object\",\n      \"description\": \"A named set of variables for request parameterization.\",\n      \"properties\": {\n        \"id\": {\"type\": \"string\"},\n        \"name\": {\"type\": \"string\"},\n        \"variables\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"key\": {\"type\": \"string\"},\n              \"value\": {\"type\": \"string\"},\n              \"enabled\": {\"type\": \"boolean\", \"default\": true}\n            },\n            \"required\": [\"key\", \"value\"]\n          }\n        }\n      },\n      \"required\": [\"name\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restfox/refs/heads/main/json-schema/restfox-collection-schema.json
tags:
- API Testing
- HTTP Client
- Browser
- Desktop
- Open Source
- GraphQL
- WebSocket
title: Restfox Collection
---
