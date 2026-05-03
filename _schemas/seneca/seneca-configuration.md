---
description: JSON Schema for Seneca microservices toolkit configuration including plugin and transport options.
layout: schema
name: Seneca Configuration
properties_list:
- description: Tag to identify this Seneca instance.
  name: tag
  type: string
- description: Default action timeout in milliseconds.
  name: timeout
  type: integer
- description: Logging configuration.
  name: log
  type: object
- description: ''
  name: debug
  type: object
- description: Plugin configurations keyed by plugin name.
  name: plugin
  type: object
- description: ''
  name: transport
  type: object
- description: Error handler function reference.
  name: errhandler
  type: string
- description: ''
  name: legacy
  type: object
provider_name: Seneca
provider_slug: seneca
schema_file: json-schema/seneca-configuration.json
slug: seneca-configuration
source_filename: seneca-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/seneca/json-schema/seneca-configuration.json\",\n  \"title\": \"Seneca Configuration\",\n  \"description\": \"JSON Schema for Seneca microservices toolkit configuration including plugin and transport options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Tag to identify this Seneca instance.\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"default\": 22222,\n      \"description\": \"Default action timeout in milliseconds.\"\n    },\n    \"log\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"enum\": [\"silent\", \"quiet\", \"any\", \"all\", \"test\", \"print\"] },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"level\": {\n              \"type\": \"string\",\n              \"enum\": [\"debug\", \"info\", \"warn\", \"error\"\
  , \"fatal\", \"none\"],\n              \"description\": \"Log level.\"\n            },\n            \"logger\": {\n              \"type\": \"string\",\n              \"description\": \"Logger implementation.\"\n            }\n          }\n        }\n      ],\n      \"description\": \"Logging configuration.\"\n    },\n    \"debug\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"undead\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Keep process alive on fatal errors.\"\n        },\n        \"short_logs\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Use shortened log output.\"\n        },\n        \"callpoint\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Include callpoint in logs.\"\n        }\n      }\n    },\n    \"plugin\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\":\
  \ \"object\",\n        \"description\": \"Plugin-specific configuration options.\"\n      },\n      \"description\": \"Plugin configurations keyed by plugin name.\"\n    },\n    \"transport\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"tcp\", \"http\", \"web\"],\n          \"default\": \"http\",\n          \"description\": \"Transport type.\"\n        },\n        \"web\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"integer\",\n              \"default\": 10101,\n              \"description\": \"HTTP port for web transport.\"\n            },\n            \"host\": {\n              \"type\": \"string\",\n              \"default\": \"0.0.0.0\",\n              \"description\": \"HTTP host for web transport.\"\n            }\n          }\n        },\n        \"tcp\": {\n          \"type\": \"object\",\n          \"properties\": {\n\
  \            \"port\": {\n              \"type\": \"integer\",\n              \"default\": 10201,\n              \"description\": \"TCP port.\"\n            },\n            \"host\": {\n              \"type\": \"string\",\n              \"default\": \"0.0.0.0\",\n              \"description\": \"TCP host.\"\n            }\n          }\n        }\n      }\n    },\n    \"errhandler\": {\n      \"type\": \"string\",\n      \"description\": \"Error handler function reference.\"\n    },\n    \"legacy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"transport\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Use legacy transport.\"\n        },\n        \"error_codes\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Use legacy error codes.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/seneca/refs/heads/main/json-schema/seneca-configuration.json
tags:
- Frameworks
- JavaScript
- Message Handling
- Microservices
- Node.js
- Pattern Matching
- Plugins
title: Seneca Configuration
---
