---
description: JSON Schema for Sentinel flow control rules used by the Dashboard API and configuration.
layout: schema
name: Alibaba Sentinel Flow Rule
properties_list: []
provider_name: Alibaba Sentinel
provider_slug: alibaba-sentinel
schema_file: json-schema/flow-rule.json
slug: flow-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/alibaba-sentinel/json-schema/flow-rule.json\",\n  \"title\": \"Alibaba Sentinel Flow Rule\",\n  \"description\": \"JSON Schema for Sentinel flow control rules used by the Dashboard API and configuration.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/$defs/FlowRule\"\n  },\n  \"$defs\": {\n    \"FlowRule\": {\n      \"type\": \"object\",\n      \"required\": [\"resource\", \"count\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the rule.\"\n        },\n        \"resource\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name to apply the flow rule to.\"\n        },\n        \"limitApp\": {\n          \"type\": \"string\",\n          \"default\": \"default\",\n          \"description\": \"Calling application to apply the rule to.\"\n  \
  \      },\n        \"grade\": {\n          \"type\": \"integer\",\n          \"enum\": [0, 1],\n          \"default\": 1,\n          \"description\": \"Threshold type: 0 = thread count, 1 = QPS.\"\n        },\n        \"count\": {\n          \"type\": \"number\",\n          \"description\": \"Threshold count value.\"\n        },\n        \"strategy\": {\n          \"type\": \"integer\",\n          \"enum\": [0, 1, 2],\n          \"default\": 0,\n          \"description\": \"Flow control strategy: 0 = direct, 1 = relate, 2 = chain.\"\n        },\n        \"refResource\": {\n          \"type\": \"string\",\n          \"description\": \"Reference resource for relate/chain strategy.\"\n        },\n        \"controlBehavior\": {\n          \"type\": \"integer\",\n          \"enum\": [0, 1, 2, 3],\n          \"default\": 0,\n          \"description\": \"Control behavior: 0 = reject directly, 1 = warm up, 2 = rate limiter, 3 = warm up + rate limiter.\"\n        },\n        \"warmUpPeriodSec\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Warm-up period in seconds for warm up behavior.\"\n        },\n        \"maxQueueingTimeMs\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum queuing time in milliseconds for rate limiter behavior.\"\n        },\n        \"clusterMode\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether the rule is for cluster flow control.\"\n        },\n        \"clusterConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"flowId\": {\n              \"type\": \"integer\",\n              \"description\": \"Cluster flow ID.\"\n            },\n            \"thresholdType\": {\n              \"type\": \"integer\",\n              \"enum\": [0, 1],\n              \"description\": \"0 = average by local, 1 = global threshold.\"\n            },\n            \"fallbackToLocalWhenFail\": {\n              \"type\": \"boolean\",\n\
  \              \"default\": true,\n              \"description\": \"Whether to fall back to local flow control on failure.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alibaba-sentinel/refs/heads/main/json-schema/flow-rule.json
tags:
- Alibaba
- Circuit Breaker
- Flow Control
- Java
- Microservices
- Rate Limiting
- Resilience
- Traffic Shaping
- Open Source
- Cloud Native
- Spring Cloud
title: Alibaba Sentinel Flow Rule
---
