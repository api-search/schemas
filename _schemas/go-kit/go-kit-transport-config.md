---
description: JSON Schema representing Go Kit service transport configuration options for HTTP, gRPC, and other transport layers, including middleware, instrumentation, and service discovery.
layout: schema
name: Go Kit Service Transport Configuration
properties_list:
- description: Service-level configuration.
  name: service
  type: object
- description: HTTP transport configuration.
  name: http
  type: object
- description: gRPC transport configuration.
  name: grpc
  type: object
- description: Service discovery configuration for client-side load balancing.
  name: serviceDiscovery
  type: object
- description: Client-side load balancer configuration.
  name: loadBalancer
  type: object
- description: Rate limiting middleware configuration.
  name: rateLimit
  type: object
- description: Circuit breaker middleware configuration.
  name: circuitBreaker
  type: object
- description: Logging middleware configuration.
  name: logging
  type: object
- description: Metrics instrumentation configuration.
  name: metrics
  type: object
- description: Distributed tracing configuration.
  name: tracing
  type: object
provider_name: Go Kit
provider_slug: go-kit
schema_file: json-schema/go-kit-transport-config.json
slug: go-kit-transport-config
source_filename: go-kit-transport-config.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/go-kit/json-schema/go-kit-transport-config.json\",\n  \"title\": \"Go Kit Service Transport Configuration\",\n  \"description\": \"JSON Schema representing Go Kit service transport configuration options for HTTP, gRPC, and other transport layers, including middleware, instrumentation, and service discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service\": {\n      \"type\": \"object\",\n      \"description\": \"Service-level configuration.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Service name for discovery and logging.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Service version.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"http\": {\n      \"type\": \"object\",\n      \"description\": \"\
  HTTP transport configuration.\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Bind address for the HTTP server.\",\n          \"default\": \":8080\"\n        },\n        \"readTimeout\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP read timeout (e.g., 30s).\",\n          \"default\": \"30s\"\n        },\n        \"writeTimeout\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP write timeout.\",\n          \"default\": \"30s\"\n        },\n        \"idleTimeout\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP idle connection timeout.\",\n          \"default\": \"120s\"\n        },\n        \"tls\": {\n          \"type\": \"object\",\n          \"description\": \"TLS configuration for the HTTP transport.\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"default\": false\n            },\n\
  \            \"certFile\": {\n              \"type\": \"string\",\n              \"description\": \"Path to TLS certificate file.\"\n            },\n            \"keyFile\": {\n              \"type\": \"string\",\n              \"description\": \"Path to TLS key file.\"\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"cors\": {\n          \"type\": \"object\",\n          \"description\": \"CORS configuration.\",\n          \"properties\": {\n            \"allowedOrigins\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" },\n              \"default\": [\"*\"]\n            },\n            \"allowedMethods\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" },\n              \"default\": [\"GET\", \"POST\", \"PUT\", \"DELETE\"]\n            },\n            \"allowedHeaders\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" }\n   \
  \         },\n            \"allowCredentials\": {\n              \"type\": \"boolean\",\n              \"default\": false\n            }\n          },\n          \"additionalProperties\": true\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"grpc\": {\n      \"type\": \"object\",\n      \"description\": \"gRPC transport configuration.\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Bind address for the gRPC server.\",\n          \"default\": \":8081\"\n        },\n        \"tls\": {\n          \"type\": \"object\",\n          \"description\": \"TLS configuration for gRPC.\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"default\": false\n            },\n            \"certFile\": {\n              \"type\": \"string\"\n            },\n            \"keyFile\": {\n              \"type\": \"string\"\n            },\n            \"caFile\"\
  : {\n              \"type\": \"string\",\n              \"description\": \"CA certificate for mutual TLS.\"\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"maxRecvMsgSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum receive message size in bytes.\",\n          \"default\": 4194304\n        },\n        \"maxSendMsgSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum send message size in bytes.\",\n          \"default\": 4194304\n        },\n        \"keepAlive\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"time\": {\n              \"type\": \"string\",\n              \"description\": \"Keepalive ping interval.\",\n              \"default\": \"2h\"\n            },\n            \"timeout\": {\n              \"type\": \"string\",\n              \"description\": \"Keepalive timeout.\",\n              \"default\": \"20s\"\n            }\n          },\n\
  \          \"additionalProperties\": true\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"serviceDiscovery\": {\n      \"type\": \"object\",\n      \"description\": \"Service discovery configuration for client-side load balancing.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Discovery mechanism.\",\n          \"enum\": [\"consul\", \"etcd\", \"eureka\", \"zookeeper\", \"dns\", \"static\"],\n          \"default\": \"consul\"\n        },\n        \"addresses\": {\n          \"type\": \"array\",\n          \"description\": \"Discovery server addresses.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"refreshInterval\": {\n          \"type\": \"string\",\n          \"description\": \"How often to refresh the service list.\",\n          \"default\": \"30s\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"loadBalancer\": {\n  \
  \    \"type\": \"object\",\n      \"description\": \"Client-side load balancer configuration.\",\n      \"properties\": {\n        \"strategy\": {\n          \"type\": \"string\",\n          \"description\": \"Load balancing strategy.\",\n          \"enum\": [\"round-robin\", \"random\", \"least-connections\"],\n          \"default\": \"round-robin\"\n        },\n        \"retryMax\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of retries.\",\n          \"default\": 3\n        },\n        \"retryTimeout\": {\n          \"type\": \"string\",\n          \"description\": \"Per-retry timeout.\",\n          \"default\": \"500ms\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"rateLimit\": {\n      \"type\": \"object\",\n      \"description\": \"Rate limiting middleware configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"requestsPerSecond\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"Maximum requests per second.\"\n        },\n        \"burst\": {\n          \"type\": \"integer\",\n          \"description\": \"Burst size for token bucket.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"circuitBreaker\": {\n      \"type\": \"object\",\n      \"description\": \"Circuit breaker middleware configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"maxRequests\": {\n          \"type\": \"integer\",\n          \"description\": \"Max requests in half-open state.\",\n          \"default\": 1\n        },\n        \"interval\": {\n          \"type\": \"string\",\n          \"description\": \"Cyclic period for clearing counts.\",\n          \"default\": \"60s\"\n        },\n        \"timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Open state timeout before transitioning\
  \ to half-open.\",\n          \"default\": \"60s\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"logging\": {\n      \"type\": \"object\",\n      \"description\": \"Logging middleware configuration.\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"enum\": [\"debug\", \"info\", \"warn\", \"error\"],\n          \"default\": \"info\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"Log format.\",\n          \"enum\": [\"logfmt\", \"json\"],\n          \"default\": \"logfmt\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Metrics instrumentation configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"Metrics\
  \ backend provider.\",\n          \"enum\": [\"prometheus\", \"statsd\", \"graphite\", \"influx\", \"dogstatsd\"],\n          \"default\": \"prometheus\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Metrics server address (for push-based backends).\"\n        },\n        \"prefix\": {\n          \"type\": \"string\",\n          \"description\": \"Metrics name prefix.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"tracing\": {\n      \"type\": \"object\",\n      \"description\": \"Distributed tracing configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"Tracing backend provider.\",\n          \"enum\": [\"zipkin\", \"jaeger\", \"lightstep\", \"opentelemetry\"],\n          \"default\": \"zipkin\"\n        },\n        \"endpoint\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Tracing collector endpoint URL.\"\n        },\n        \"sampleRate\": {\n          \"type\": \"number\",\n          \"description\": \"Sampling rate (0.0 - 1.0).\",\n          \"default\": 1.0,\n          \"minimum\": 0.0,\n          \"maximum\": 1.0\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/go-kit/refs/heads/main/json-schema/go-kit-transport-config.json
tags:
- Distributed Systems
- Domain-Driven Design
- Frameworks
- Go
- Golang
- Microservices
title: Go Kit Service Transport Configuration
---
