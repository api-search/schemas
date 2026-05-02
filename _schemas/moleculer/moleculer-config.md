---
description: JSON Schema for the moleculer.config.js broker configuration file, covering transporter, serializer, cacher, logger, metrics, tracing, and other broker options.
layout: schema
name: Moleculer Broker Configuration
properties_list:
- description: Namespace for node segmentation.
  name: namespace
  type: string
- description: Unique node identifier. Auto-generated if not set.
  name: nodeID
  type: string
- description: Custom metadata for the node.
  name: metadata
  type: object
- description: Logger configuration. Can be boolean, string, object, or array.
  name: logger
  type: object
- description: Transporter for inter-node communication.
  name: transporter
  type: object
- description: Cacher configuration for action results.
  name: cacher
  type: object
- description: Serializer for message encoding.
  name: serializer
  type: object
- description: Request timeout in milliseconds (0 = disabled).
  name: requestTimeout
  type: integer
- description: Retry policy for failed requests.
  name: retryPolicy
  type: object
- description: Clone context params for safety.
  name: contextParamsCloning
  type: boolean
- description: Maximum nested call level to prevent infinite loops.
  name: maxCallLevel
  type: integer
- description: Heartbeat interval in seconds.
  name: heartbeatInterval
  type: integer
- description: Heartbeat timeout in seconds.
  name: heartbeatTimeout
  type: integer
- description: Request tracking and graceful shutdown configuration.
  name: tracking
  type: object
- description: Disable built-in request balancer (for transporter balancing).
  name: disableBalancer
  type: boolean
- description: Service registry options.
  name: registry
  type: object
- description: Circuit breaker configuration.
  name: circuitBreaker
  type: object
- description: Bulkhead configuration for concurrency limiting.
  name: bulkhead
  type: object
- description: Parameter validator.
  name: validator
  type: object
- description: Global error handler function name.
  name: errorHandler
  type: string
- description: Metrics configuration.
  name: metrics
  type: object
- description: Distributed tracing configuration.
  name: tracing
  type: object
- description: List of middleware to load.
  name: middlewares
  type: array
- description: Custom REPL commands.
  name: replCommands
  type: array
provider_name: Moleculer
provider_slug: moleculer
schema_file: json-schema/moleculer-config.json
slug: moleculer-config
source_filename: moleculer-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/moleculer/json-schema/moleculer-config.json\",\n  \"title\": \"Moleculer Broker Configuration\",\n  \"description\": \"JSON Schema for the moleculer.config.js broker configuration file, covering transporter, serializer, cacher, logger, metrics, tracing, and other broker options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace for node segmentation.\",\n      \"default\": \"\"\n    },\n    \"nodeID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique node identifier. Auto-generated if not set.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata for the node.\",\n      \"additionalProperties\": true\n    },\n    \"logger\": {\n      \"description\": \"Logger configuration. Can be boolean, string, object, or array.\"\
  ,\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        { \"type\": \"string\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"Logger type.\",\n              \"enum\": [\"Console\", \"File\", \"Pino\", \"Bunyan\", \"Winston\", \"Debug\", \"Log4js\"]\n            },\n            \"options\": {\n              \"type\": \"object\",\n              \"description\": \"Logger-specific options.\",\n              \"properties\": {\n                \"level\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"trace\", \"debug\", \"info\", \"warn\", \"error\", \"fatal\"],\n                  \"default\": \"info\"\n                },\n                \"colors\": {\n                  \"type\": \"boolean\",\n                  \"default\": true\n                },\n                \"moduleColors\": {\n                  \"type\": \"boolean\",\n \
  \                 \"default\": false\n                },\n                \"formatter\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"full\", \"short\", \"simple\"]\n                },\n                \"autoPadding\": {\n                  \"type\": \"boolean\",\n                  \"default\": false\n                }\n              },\n              \"additionalProperties\": true\n            }\n          }\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      ]\n    },\n    \"transporter\": {\n      \"description\": \"Transporter for inter-node communication.\",\n      \"oneOf\": [\n        { \"type\": \"string\", \"description\": \"Connection string (e.g., nats://localhost:4222, redis://localhost:6379).\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Transporter type.\",\n              \"enum\": [\"NATS\", \"Redis\", \"MQTT\", \"AMQP\", \"AMQP10\", \"STAN\", \"Kafka\", \"TCP\"]\n            },\n            \"options\": {\n              \"type\": \"object\",\n              \"description\": \"Transporter-specific options.\",\n              \"additionalProperties\": true\n            }\n          }\n        },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"cacher\": {\n      \"description\": \"Cacher configuration for action results.\",\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        { \"type\": \"string\" },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"Memory\", \"MemoryLRU\", \"Redis\", \"RedisSentinel\"]\n            },\n            \"options\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"ttl\": {\n                  \"type\": \"integer\",\n\
  \                  \"description\": \"Default TTL in seconds.\",\n                  \"default\": 30\n                },\n                \"maxParamsLength\": {\n                  \"type\": \"integer\",\n                  \"default\": 100\n                },\n                \"redis\": {\n                  \"type\": \"string\",\n                  \"description\": \"Redis connection string.\"\n                }\n              },\n              \"additionalProperties\": true\n            }\n          }\n        },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"serializer\": {\n      \"description\": \"Serializer for message encoding.\",\n      \"oneOf\": [\n        { \"type\": \"string\", \"enum\": [\"JSON\", \"Avro\", \"MsgPack\", \"Notepack\", \"ProtoBuf\", \"Thrift\", \"CBOR\"] },\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\"\n            },\n            \"options\": {\n              \"type\"\
  : \"object\",\n              \"additionalProperties\": true\n            }\n          }\n        },\n        { \"type\": \"null\" }\n      ],\n      \"default\": \"JSON\"\n    },\n    \"requestTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Request timeout in milliseconds (0 = disabled).\",\n      \"default\": 0\n    },\n    \"retryPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Retry policy for failed requests.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"retries\": {\n          \"type\": \"integer\",\n          \"default\": 5\n        },\n        \"delay\": {\n          \"type\": \"integer\",\n          \"description\": \"Initial delay in milliseconds.\",\n          \"default\": 100\n        },\n        \"maxDelay\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum delay in milliseconds.\",\n          \"default\": 1000\n      \
  \  },\n        \"factor\": {\n          \"type\": \"number\",\n          \"description\": \"Backoff factor.\",\n          \"default\": 2\n        },\n        \"check\": {\n          \"type\": \"string\",\n          \"description\": \"Error check function expression.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"contextParamsCloning\": {\n      \"type\": \"boolean\",\n      \"description\": \"Clone context params for safety.\",\n      \"default\": false\n    },\n    \"maxCallLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum nested call level to prevent infinite loops.\",\n      \"default\": 0\n    },\n    \"heartbeatInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Heartbeat interval in seconds.\",\n      \"default\": 10\n    },\n    \"heartbeatTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Heartbeat timeout in seconds.\",\n      \"default\": 30\n    },\n    \"tracking\": {\n      \"type\":\
  \ \"object\",\n      \"description\": \"Request tracking and graceful shutdown configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"shutdownTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Shutdown timeout in milliseconds.\",\n          \"default\": 5000\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"disableBalancer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Disable built-in request balancer (for transporter balancing).\",\n      \"default\": false\n    },\n    \"registry\": {\n      \"type\": \"object\",\n      \"description\": \"Service registry options.\",\n      \"properties\": {\n        \"strategy\": {\n          \"type\": \"string\",\n          \"description\": \"Load balancing strategy.\",\n          \"enum\": [\"RoundRobin\", \"Random\", \"CpuUsage\", \"Latency\", \"Shard\"],\n          \"default\": \"RoundRobin\"\
  \n        },\n        \"preferLocal\": {\n          \"type\": \"boolean\",\n          \"default\": true\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"circuitBreaker\": {\n      \"type\": \"object\",\n      \"description\": \"Circuit breaker configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"threshold\": {\n          \"type\": \"number\",\n          \"description\": \"Failure rate threshold (0.0 - 1.0).\",\n          \"default\": 0.5\n        },\n        \"minRequestCount\": {\n          \"type\": \"integer\",\n          \"default\": 20\n        },\n        \"windowTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Time window in seconds.\",\n          \"default\": 60\n        },\n        \"halfOpenTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Half-open state duration in milliseconds.\",\n          \"default\"\
  : 10000\n        },\n        \"check\": {\n          \"type\": \"string\",\n          \"description\": \"Error check function expression.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"bulkhead\": {\n      \"type\": \"object\",\n      \"description\": \"Bulkhead configuration for concurrency limiting.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"concurrency\": {\n          \"type\": \"integer\",\n          \"default\": 10\n        },\n        \"maxQueueSize\": {\n          \"type\": \"integer\",\n          \"default\": 100\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"validator\": {\n      \"description\": \"Parameter validator.\",\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        { \"type\": \"string\" },\n        { \"type\": \"object\" }\n      ],\n      \"default\": true\n    },\n    \"errorHandler\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Global error handler function name.\"\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Metrics configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"reporter\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"Console\", \"CSV\", \"Datadog\", \"Event\", \"Prometheus\", \"StatsD\"]\n                },\n                \"options\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": true\n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"object\" }\n            }\n          ]\n        }\n   \
  \   },\n      \"additionalProperties\": true\n    },\n    \"tracing\": {\n      \"type\": \"object\",\n      \"description\": \"Distributed tracing configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"exporter\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"Console\", \"Datadog\", \"Event\", \"EventLegacy\", \"Jaeger\", \"Zipkin\", \"NewRelic\"]\n                },\n                \"options\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": true\n                }\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"object\" }\n            }\n          ]\n        }\n      },\n\
  \      \"additionalProperties\": true\n    },\n    \"middlewares\": {\n      \"type\": \"array\",\n      \"description\": \"List of middleware to load.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"replCommands\": {\n      \"type\": \"array\",\n      \"description\": \"Custom REPL commands.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moleculer/refs/heads/main/json-schema/moleculer-config.json
tags:
- Fault Tolerance
- Frameworks
- JavaScript
- Load Balancing
- Microservices
- Node.js
- Service Discovery
title: Moleculer Broker Configuration
---
