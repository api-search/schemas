---
description: Describes a microservice in a scalable architecture, including its service boundaries, communication contracts, resource requirements, and operational characteristics.
layout: schema
name: Microservice
properties_list:
- description: Service name in kebab-case.
  name: name
  type: string
- description: Semantic version of the service.
  name: version
  type: string
- description: Human-readable description of the service's bounded context and responsibilities.
  name: description
  type: string
- description: Team responsible for this service (follows domain-driven team ownership).
  name: team
  type: string
- description: Domain or bounded context this service belongs to.
  name: domain
  type: string
- description: Service API contract definition.
  name: api
  type: object
- description: List of upstream services this service depends on.
  name: dependencies
  type: array
- description: ''
  name: resources
  type: object
- description: ''
  name: scaling
  type: object
- description: ''
  name: resilience
  type: object
- description: ''
  name: observability
  type: object
- description: ''
  name: tags
  type: array
provider_name: Scalable Architecture
provider_slug: scalable-architecture
schema_file: json-schema/scalable-architecture-microservice-schema.json
slug: scalable-architecture-microservice
source_filename: scalable-architecture-microservice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-architecture/main/json-schema/scalable-architecture-microservice-schema.json\",\n  \"title\": \"Microservice\",\n  \"description\": \"Describes a microservice in a scalable architecture, including its service boundaries, communication contracts, resource requirements, and operational characteristics.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"version\", \"api\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name in kebab-case.\",\n      \"pattern\": \"^[a-z][a-z0-9-]*$\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Semantic version of the service.\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+(-[a-zA-Z0-9.]+)?$\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description\
  \ of the service's bounded context and responsibilities.\"\n    },\n    \"team\": {\n      \"type\": \"string\",\n      \"description\": \"Team responsible for this service (follows domain-driven team ownership).\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain or bounded context this service belongs to.\"\n    },\n    \"api\": {\n      \"type\": \"object\",\n      \"description\": \"Service API contract definition.\",\n      \"required\": [\"protocol\"],\n      \"properties\": {\n        \"protocol\": {\n          \"type\": \"string\",\n          \"enum\": [\"HTTP/REST\", \"gRPC\", \"GraphQL\", \"WebSocket\", \"AMQP\", \"Kafka\"],\n          \"description\": \"Primary communication protocol.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"API version (e.g., v1, v2).\",\n          \"default\": \"v1\"\n        },\n        \"baseUrl\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uri\",\n          \"description\": \"Base URL for the service API.\"\n        },\n        \"healthEndpoint\": {\n          \"type\": \"string\",\n          \"description\": \"Health check endpoint path.\",\n          \"default\": \"/health\"\n        },\n        \"metricsEndpoint\": {\n          \"type\": \"string\",\n          \"description\": \"Prometheus metrics endpoint path.\",\n          \"default\": \"/metrics\"\n        }\n      }\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"List of upstream services this service depends on.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"name\", \"type\"],\n        \"properties\": {\n          \"name\": {\"type\": \"string\"},\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"synchronous\", \"asynchronous\", \"database\", \"cache\", \"queue\"]\n          },\n          \"required\": {\"type\": \"boolean\", \"default\": true},\n          \"\
  circuitBreaker\": {\"type\": \"boolean\", \"default\": false}\n        }\n      }\n    },\n    \"resources\": {\n      \"$ref\": \"#/$defs/ResourceRequirements\"\n    },\n    \"scaling\": {\n      \"$ref\": \"#/$defs/ScalingConfig\"\n    },\n    \"resilience\": {\n      \"$ref\": \"#/$defs/ResilienceConfig\"\n    },\n    \"observability\": {\n      \"$ref\": \"#/$defs/ObservabilityConfig\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"}\n    }\n  },\n  \"$defs\": {\n    \"ResourceRequirements\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes-style resource requests and limits.\",\n      \"properties\": {\n        \"requests\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cpu\": {\"type\": \"string\", \"description\": \"CPU request (e.g., '100m', '0.5').\"},\n            \"memory\": {\"type\": \"string\", \"description\": \"Memory request (e.g., '128Mi', '1Gi').\"}\n          }\n       \
  \ },\n        \"limits\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cpu\": {\"type\": \"string\"},\n            \"memory\": {\"type\": \"string\"}\n          }\n        }\n      }\n    },\n    \"ScalingConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Autoscaling configuration for the service.\",\n      \"properties\": {\n        \"minReplicas\": {\"type\": \"integer\", \"minimum\": 0, \"default\": 1},\n        \"maxReplicas\": {\"type\": \"integer\", \"minimum\": 1},\n        \"targetCPUUtilizationPercentage\": {\"type\": \"integer\", \"minimum\": 1, \"maximum\": 100},\n        \"scaleToZero\": {\"type\": \"boolean\", \"default\": false},\n        \"scalingTrigger\": {\n          \"type\": \"string\",\n          \"enum\": [\"cpu\", \"memory\", \"custom-metric\", \"queue-depth\", \"event-driven\"]\n        }\n      }\n    },\n    \"ResilienceConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Resilience patterns applied\
  \ to the service.\",\n      \"properties\": {\n        \"circuitBreaker\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\"type\": \"boolean\", \"default\": false},\n            \"threshold\": {\"type\": \"number\", \"minimum\": 0, \"maximum\": 1},\n            \"timeout\": {\"type\": \"integer\", \"description\": \"Recovery timeout in seconds.\"}\n          }\n        },\n        \"retry\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\"type\": \"boolean\", \"default\": false},\n            \"maxAttempts\": {\"type\": \"integer\", \"minimum\": 1, \"default\": 3},\n            \"backoff\": {\n              \"type\": \"string\",\n              \"enum\": [\"fixed\", \"exponential\", \"jitter\"],\n              \"default\": \"exponential\"\n            }\n          }\n        },\n        \"timeout\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"requestTimeoutMs\": {\"\
  type\": \"integer\", \"minimum\": 0},\n            \"connectionTimeoutMs\": {\"type\": \"integer\", \"minimum\": 0}\n          }\n        }\n      }\n    },\n    \"ObservabilityConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Observability instrumentation settings.\",\n      \"properties\": {\n        \"tracingEnabled\": {\"type\": \"boolean\", \"default\": true},\n        \"metricsEnabled\": {\"type\": \"boolean\", \"default\": true},\n        \"loggingLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"DEBUG\", \"INFO\", \"WARN\", \"ERROR\"],\n          \"default\": \"INFO\"\n        },\n        \"samplingRate\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"description\": \"Distributed trace sampling rate (0.0-1.0).\",\n          \"default\": 0.1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-architecture/refs/heads/main/json-schema/scalable-architecture-microservice-schema.json
tags:
- Cloud Architecture
- Cloud Native
- Distributed Systems
- High Availability
- Infrastructure
- Microservices
- Performance
- Resilience
- Scalability
- Service Mesh
title: Microservice
---
