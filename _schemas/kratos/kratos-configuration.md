---
description: JSON Schema for Kratos microservice framework configuration (kratos.yaml / config.yaml).
layout: schema
name: Kratos Service Configuration
properties_list:
- description: ''
  name: server
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: registry
  type: object
- description: ''
  name: trace
  type: object
- description: ''
  name: log
  type: object
provider_name: Kratos
provider_slug: kratos
schema_file: json-schema/kratos-configuration.json
slug: kratos-configuration
source_filename: kratos-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kratos/json-schema/kratos-configuration.json\",\n  \"title\": \"Kratos Service Configuration\",\n  \"description\": \"JSON Schema for Kratos microservice framework configuration (kratos.yaml / config.yaml).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"server\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"http\": {\n          \"$ref\": \"#/$defs/ServerConfig\"\n        },\n        \"grpc\": {\n          \"$ref\": \"#/$defs/ServerConfig\"\n        }\n      }\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"database\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"driver\": {\n              \"type\": \"string\",\n              \"description\": \"Database driver name.\"\n            },\n            \"source\": {\n              \"type\": \"string\",\n       \
  \       \"description\": \"Database connection string.\"\n            }\n          }\n        },\n        \"redis\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"addr\": {\n              \"type\": \"string\",\n              \"description\": \"Redis server address.\"\n            },\n            \"dial_timeout\": {\n              \"type\": \"string\",\n              \"description\": \"Dial timeout duration.\"\n            },\n            \"read_timeout\": {\n              \"type\": \"string\",\n              \"description\": \"Read timeout duration.\"\n            },\n            \"write_timeout\": {\n              \"type\": \"string\",\n              \"description\": \"Write timeout duration.\"\n            }\n          }\n        }\n      }\n    },\n    \"registry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"consul\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"address\": {\n              \"\
  type\": \"string\",\n              \"description\": \"Consul server address.\"\n            },\n            \"scheme\": {\n              \"type\": \"string\",\n              \"default\": \"http\"\n            }\n          }\n        },\n        \"etcd\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"endpoints\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" },\n              \"description\": \"Etcd endpoints.\"\n            }\n          }\n        }\n      }\n    },\n    \"trace\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"description\": \"Tracing collector endpoint.\"\n        },\n        \"sampler\": {\n          \"type\": \"number\",\n          \"description\": \"Sampling rate (0.0 to 1.0).\"\n        }\n      }\n    },\n    \"log\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"level\": {\n          \"type\"\
  : \"string\",\n          \"enum\": [\"DEBUG\", \"INFO\", \"WARN\", \"ERROR\", \"FATAL\"],\n          \"description\": \"Log level.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"ServerConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"addr\": {\n          \"type\": \"string\",\n          \"description\": \"Server listen address (e.g., 0.0.0.0:8000).\"\n        },\n        \"timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Server timeout duration.\"\n        },\n        \"middleware\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"logging\": {\n              \"type\": \"boolean\",\n              \"description\": \"Enable logging middleware.\"\n            },\n            \"recovery\": {\n              \"type\": \"boolean\",\n              \"description\": \"Enable recovery middleware.\"\n            },\n            \"tracing\": {\n              \"type\": \"boolean\",\n              \"description\"\
  : \"Enable tracing middleware.\"\n            },\n            \"metrics\": {\n              \"type\": \"boolean\",\n              \"description\": \"Enable metrics middleware.\"\n            }\n          }\n        },\n        \"tls\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cert_file\": {\n              \"type\": \"string\",\n              \"description\": \"Path to TLS certificate file.\"\n            },\n            \"key_file\": {\n              \"type\": \"string\",\n              \"description\": \"Path to TLS key file.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kratos/refs/heads/main/json-schema/kratos-configuration.json
tags:
- Cloud Native
- Frameworks
- Go
- gRPC
- Microservices
- Protocol Buffers
- Service Discovery
title: Kratos Service Configuration
---
