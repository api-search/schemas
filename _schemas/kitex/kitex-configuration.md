---
description: JSON Schema for Kitex RPC framework service configuration including client and server options.
layout: schema
name: Kitex Service Configuration
properties_list:
- description: ''
  name: server
  type: object
- description: ''
  name: client
  type: object
- description: ''
  name: registry
  type: object
provider_name: Kitex
provider_slug: kitex
schema_file: json-schema/kitex-configuration.json
slug: kitex-configuration
source_filename: kitex-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kitex/json-schema/kitex-configuration.json\",\n  \"title\": \"Kitex Service Configuration\",\n  \"description\": \"JSON Schema for Kitex RPC framework service configuration including client and server options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"server\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"service_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the service.\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Server listen address (e.g., :8888).\"\n        },\n        \"exit_wait_time\": {\n          \"type\": \"string\",\n          \"description\": \"Grace period before server exits.\"\n        },\n        \"max_connections\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of connections.\"\n  \
  \      },\n        \"mux_transport\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Enable multiplexed transport.\"\n        },\n        \"read_write_timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Read/write timeout duration.\"\n        },\n        \"limit\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"max_connections\": {\n              \"type\": \"integer\",\n              \"description\": \"Connection limit.\"\n            },\n            \"max_qps\": {\n              \"type\": \"integer\",\n              \"description\": \"QPS limit.\"\n            },\n            \"update_interval\": {\n              \"type\": \"string\",\n              \"description\": \"Interval for updating limiter.\"\n            }\n          }\n        }\n      }\n    },\n    \"client\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"rpc_timeout\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"RPC timeout duration.\"\n        },\n        \"connect_timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Connection timeout duration.\"\n        },\n        \"retry\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"max_retry_times\": {\n              \"type\": \"integer\",\n              \"default\": 2,\n              \"description\": \"Maximum retry attempts.\"\n            },\n            \"ee_retry\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\": \"boolean\" },\n                \"max_retry_times\": { \"type\": \"integer\" },\n                \"retry_delay\": { \"type\": \"string\" }\n              },\n              \"description\": \"Error-based retry configuration.\"\n            },\n            \"backup_request\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\"\
  : \"boolean\" },\n                \"retry_delay\": { \"type\": \"string\" }\n              },\n              \"description\": \"Backup request (hedging) configuration.\"\n            }\n          }\n        },\n        \"circuit_breaker\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"default\": true,\n              \"description\": \"Enable circuit breaker.\"\n            },\n            \"error_rate\": {\n              \"type\": \"number\",\n              \"description\": \"Error rate threshold.\"\n            },\n            \"min_sample\": {\n              \"type\": \"integer\",\n              \"description\": \"Minimum sample count.\"\n            }\n          }\n        },\n        \"loadbalancer\": {\n          \"type\": \"string\",\n          \"enum\": [\"weight_round_robin\", \"random\", \"round_robin\", \"interleaved_weighted_round_robin\", \"alias_method\"],\n          \"description\"\
  : \"Load balancing algorithm.\"\n        }\n      }\n    },\n    \"registry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"etcd\", \"consul\", \"nacos\", \"polaris\", \"zookeeper\"],\n          \"description\": \"Service registry type.\"\n        },\n        \"address\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Registry server addresses.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kitex/refs/heads/main/json-schema/kitex-configuration.json
tags:
- Frameworks
- Go
- High Performance
- Microservices
- Protocol Buffers
- RPC
- Thrift
title: Kitex Service Configuration
---
