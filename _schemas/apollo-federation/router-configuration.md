---
description: JSON Schema for Apollo Router configuration (router.yaml).
layout: schema
name: Apollo Router Configuration
properties_list:
- description: ''
  name: supergraph
  type: object
- description: ''
  name: cors
  type: object
- description: ''
  name: headers
  type: object
- description: ''
  name: telemetry
  type: object
- description: ''
  name: traffic_shaping
  type: object
- description: ''
  name: limits
  type: object
- description: ''
  name: sandbox
  type: object
- description: ''
  name: homepage
  type: object
provider_name: Apollo Federation
provider_slug: apollo-federation
schema_file: json-schema/router-configuration.json
slug: router-configuration
source_filename: router-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apollo-federation/json-schema/router-configuration.json\",\n  \"title\": \"Apollo Router Configuration\",\n  \"description\": \"JSON Schema for Apollo Router configuration (router.yaml).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"supergraph\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"listen\": {\n          \"type\": \"string\",\n          \"default\": \"127.0.0.1:4000\",\n          \"description\": \"Address the router listens on.\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"default\": \"/\",\n          \"description\": \"Path for the GraphQL endpoint.\"\n        },\n        \"introspection\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Enable GraphQL introspection.\"\n        }\n      }\n    },\n    \"cors\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"origins\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Allowed CORS origins.\"\n        },\n        \"allow_any_origin\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Allow any origin.\"\n        },\n        \"methods\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"allow_headers\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"all\": {\n          \"$ref\": \"#/$defs/HeaderRules\"\n        },\n        \"subgraphs\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/HeaderRules\"\n          }\n        }\n      }\n    },\n    \"telemetry\": {\n      \"type\": \"object\",\n \
  \     \"properties\": {\n        \"apollo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"endpoint\": { \"type\": \"string\" },\n            \"apollo_key\": { \"type\": \"string\" },\n            \"apollo_graph_ref\": { \"type\": \"string\" }\n          }\n        },\n        \"tracing\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"trace_config\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"service_name\": { \"type\": \"string\" },\n                \"sampler\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"always_on\", \"always_off\"]\n                }\n              }\n            },\n            \"otlp\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\": \"boolean\" },\n                \"endpoint\": { \"type\": \"string\" },\n                \"protocol\": {\n                  \"\
  type\": \"string\",\n                  \"enum\": [\"grpc\", \"http\"]\n                }\n              }\n            },\n            \"jaeger\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\": \"boolean\" },\n                \"agent\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"endpoint\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"metrics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"prometheus\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\": \"boolean\", \"default\": false },\n                \"listen\": { \"type\": \"string\" },\n                \"path\": { \"type\": \"string\", \"default\": \"/metrics\" }\n              }\n            }\n          }\n        }\n   \
  \   }\n    },\n    \"traffic_shaping\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"all\": {\n          \"$ref\": \"#/$defs/TrafficShapingConfig\"\n        },\n        \"subgraphs\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TrafficShapingConfig\"\n          }\n        },\n        \"router\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"timeout\": { \"type\": \"string\" },\n            \"global_rate_limit\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"capacity\": { \"type\": \"integer\" },\n                \"interval\": { \"type\": \"string\" }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"limits\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"max_depth\": { \"type\": \"integer\", \"description\": \"Maximum query depth.\" },\n        \"max_height\": { \"type\": \"\
  integer\", \"description\": \"Maximum query height.\" },\n        \"max_aliases\": { \"type\": \"integer\", \"description\": \"Maximum number of aliases.\" },\n        \"max_root_fields\": { \"type\": \"integer\", \"description\": \"Maximum root fields.\" },\n        \"parser_max_tokens\": { \"type\": \"integer\" },\n        \"parser_max_recursion\": { \"type\": \"integer\" }\n      }\n    },\n    \"sandbox\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Enable Apollo Sandbox explorer.\"\n        }\n      }\n    },\n    \"homepage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Enable the router homepage.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"HeaderRules\": {\n      \"type\": \"object\",\n      \"properties\": {\n\
  \        \"request\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"propagate\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"named\": { \"type\": \"string\" },\n                  \"matching\": { \"type\": \"string\" },\n                  \"rename\": { \"type\": \"string\" },\n                  \"default\": { \"type\": \"string\" }\n                }\n              },\n              \"remove\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"named\": { \"type\": \"string\" },\n                  \"matching\": { \"type\": \"string\" }\n                }\n              },\n              \"insert\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": { \"type\": \"string\" },\n                  \"value\": { \"type\": \"string\" }\n             \
  \   }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"TrafficShapingConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Request timeout duration.\"\n        },\n        \"deduplicate_query\": {\n          \"type\": \"boolean\",\n          \"default\": true,\n          \"description\": \"Enable query deduplication.\"\n        },\n        \"compression\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Enable response compression.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apollo-federation/refs/heads/main/json-schema/router-configuration.json
tags:
- API Gateway
- Federation
- GraphQL
- Microservices
- Open Source
- Subgraphs
- Supergraph
title: Apollo Router Configuration
---
