---
description: Connector schema from Ballerina Central API
layout: schema
name: Connector
properties_list:
- description: ''
  name: organization
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: readme
  type: string
- description: ''
  name: functions
  type: array
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-connector-schema.json
slug: central-api-connector
source_filename: central-api-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-connector-schema.json\",\n  \"title\": \"Connector\",\n  \"description\": \"Connector schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organization\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    },\n    \"readme\": {\n      \"type\": \"string\"\n    },\n    \"functions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"parameters\"\
  : {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"type\": {\n                  \"type\": \"string\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\n                },\n                \"defaultValue\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"returnType\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-connector-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: Connector
---
