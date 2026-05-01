---
description: JSON Schema for the encore.app configuration file that defines an Encore application.
layout: schema
name: Encore App Configuration
properties_list:
- description: Unique application ID from the Encore platform.
  name: id
  type: string
- description: Primary programming language for the application.
  name: lang
  type: string
- description: ''
  name: global_cors
  type: object
- description: List of experimental features to enable.
  name: experiments
  type: array
- description: ''
  name: build
  type: object
- description: ''
  name: generate
  type: object
provider_name: Encore
provider_slug: encore
schema_file: json-schema/encore-app-configuration.json
slug: encore-app-configuration
source_filename: encore-app-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/encore/json-schema/encore-app-configuration.json\",\n  \"title\": \"Encore App Configuration\",\n  \"description\": \"JSON Schema for the encore.app configuration file that defines an Encore application.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique application ID from the Encore platform.\"\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"enum\": [\"go\", \"typescript\"],\n      \"description\": \"Primary programming language for the application.\"\n    },\n    \"global_cors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"allow_origins_without_credentials\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Origins allowed without credentials.\"\n        },\n\
  \        \"allow_origins_with_credentials\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Origins allowed with credentials.\"\n        },\n        \"debug\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Enable CORS debug mode.\"\n        }\n      }\n    },\n    \"experiments\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"List of experimental features to enable.\"\n    },\n    \"build\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"docker\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bundle_source\": {\n              \"type\": \"boolean\",\n              \"default\": false,\n              \"description\": \"Whether to bundle source code in Docker image.\"\n            },\n            \"base_image\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Custom base Docker image.\"\n            }\n          }\n        }\n      }\n    },\n    \"generate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"typescript\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"output\": {\n              \"type\": \"string\",\n              \"description\": \"Output directory for generated TypeScript client.\"\n            }\n          }\n        },\n        \"go\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"output\": {\n              \"type\": \"string\",\n              \"description\": \"Output directory for generated Go client.\"\n            }\n          }\n        },\n        \"openapi\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"output\": {\n              \"type\": \"string\",\n              \"description\": \"Output directory for generated OpenAPI spec.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/encore/refs/heads/main/json-schema/encore-app-configuration.json
tags:
- Backend
- Cloud Native
- Frameworks
- Go
- Infrastructure Automation
- Microservices
- Open Source
- TypeScript
title: Encore App Configuration
---
