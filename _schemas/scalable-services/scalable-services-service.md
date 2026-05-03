---
description: Schema representing a scalable cloud service with configuration for scaling, load balancing, health checks, and observability.
layout: schema
name: Scalable Service
properties_list:
- description: Human-readable name of the service.
  name: name
  type: string
- description: The type of scalable service.
  name: type
  type: string
- description: Base URL of the service API.
  name: baseUrl
  type: string
- description: Relative path for health/readiness check endpoint.
  name: healthEndpoint
  type: string
- description: Relative path for Prometheus-compatible metrics endpoint.
  name: metricsEndpoint
  type: string
- description: Auto-scaling configuration for the service.
  name: scalingPolicy
  type: object
- description: Load balancing configuration.
  name: loadBalancing
  type: object
- description: Rate limiting configuration.
  name: rateLimiting
  type: object
- description: Circuit breaker configuration for fault tolerance.
  name: circuitBreaker
  type: object
- description: Observability configuration.
  name: observability
  type: object
- description: Classification tags for the service.
  name: tags
  type: array
provider_name: Scalable Services
provider_slug: scalable-services
schema_file: json-schema/scalable-services-service-schema.json
slug: scalable-services-service
source_filename: scalable-services-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.com/schemas/scalable-services/service\",\n  \"title\": \"Scalable Service\",\n  \"description\": \"Schema representing a scalable cloud service with configuration for scaling, load balancing, health checks, and observability.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\", \"baseUrl\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the service.\",\n      \"example\": \"Payment Processing Service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"microservice\", \"serverless\", \"container\", \"api-gateway\", \"service-mesh\", \"load-balancer\"],\n      \"description\": \"The type of scalable service.\"\n    },\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL of the service API.\"\n    },\n    \"healthEndpoint\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Relative path for health/readiness check endpoint.\",\n      \"example\": \"/healthz\"\n    },\n    \"metricsEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"Relative path for Prometheus-compatible metrics endpoint.\",\n      \"example\": \"/metrics\"\n    },\n    \"scalingPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-scaling configuration for the service.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"horizontal\", \"vertical\", \"both\"],\n          \"description\": \"Scaling axis.\"\n        },\n        \"minReplicas\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Minimum number of running replicas (0 = scale to zero).\"\n        },\n        \"maxReplicas\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum number of replicas.\"\
  \n        },\n        \"targetCPUPercent\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 100,\n          \"description\": \"Target CPU utilization percentage for horizontal scaling trigger.\"\n        },\n        \"scaleToZero\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the service can scale to zero replicas when idle (serverless).\"\n        }\n      }\n    },\n    \"loadBalancing\": {\n      \"type\": \"object\",\n      \"description\": \"Load balancing configuration.\",\n      \"properties\": {\n        \"algorithm\": {\n          \"type\": \"string\",\n          \"enum\": [\"round-robin\", \"least-connections\", \"ip-hash\", \"random\", \"weighted\"],\n          \"description\": \"Load balancing algorithm.\"\n        },\n        \"healthCheckIntervalSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Interval in seconds between health checks.\"\n        },\n        \"stickySession\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"Whether session affinity (sticky sessions) is enabled.\"\n        }\n      }\n    },\n    \"rateLimiting\": {\n      \"type\": \"object\",\n      \"description\": \"Rate limiting configuration.\",\n      \"properties\": {\n        \"requestsPerSecond\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum requests per second per client.\"\n        },\n        \"requestsPerMinute\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum requests per minute per client.\"\n        },\n        \"strategy\": {\n          \"type\": \"string\",\n          \"enum\": [\"token-bucket\", \"sliding-window\", \"fixed-window\"],\n          \"description\": \"Rate limiting algorithm.\"\n        }\n      }\n    },\n    \"circuitBreaker\": {\n      \"type\": \"object\",\n      \"description\": \"Circuit breaker configuration for fault tolerance.\",\n      \"properties\": {\n        \"enabled\": {\n\
  \          \"type\": \"boolean\"\n        },\n        \"failureThreshold\": {\n          \"type\": \"number\",\n          \"description\": \"Failure rate (0-1) at which circuit opens.\"\n        },\n        \"timeoutSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Time circuit remains open before half-open probe.\"\n        }\n      }\n    },\n    \"observability\": {\n      \"type\": \"object\",\n      \"description\": \"Observability configuration.\",\n      \"properties\": {\n        \"tracingEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"tracingBackend\": {\n          \"type\": \"string\",\n          \"enum\": [\"jaeger\", \"zipkin\", \"opentelemetry\", \"datadog\", \"honeycomb\"],\n          \"description\": \"Distributed tracing backend.\"\n        },\n        \"loggingFormat\": {\n          \"type\": \"string\",\n          \"enum\": [\"json\", \"logfmt\", \"text\"],\n          \"description\": \"Structured logging format.\"\n   \
  \     }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Classification tags for the service.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-services/refs/heads/main/json-schema/scalable-services-service-schema.json
tags:
- API Gateway
- Cloud Native
- Containers
- Distributed Systems
- High Availability
- Kubernetes
- Load Balancing
- Microservices
- Scalable Architecture
- Serverless
- Service Mesh
title: Scalable Service
---
