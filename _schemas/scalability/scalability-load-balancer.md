---
description: Describes a load balancer configuration for distributing network traffic across multiple compute resources to ensure high availability and scalability.
layout: schema
name: Load Balancer
properties_list:
- description: Unique identifier for the load balancer.
  name: id
  type: string
- description: Human-readable name for the load balancer.
  name: name
  type: string
- description: Layer at which the load balancer operates.
  name: type
  type: string
- description: Traffic distribution algorithm.
  name: algorithm
  type: string
- description: Network protocol.
  name: protocol
  type: string
- description: Port on which the load balancer listens for incoming traffic.
  name: frontendPort
  type: integer
- description: ''
  name: healthCheck
  type: object
- description: List of backend targets receiving distributed traffic.
  name: backends
  type: array
- description: Session affinity/persistence configuration.
  name: stickySession
  type: object
- description: Whether TLS is terminated at the load balancer.
  name: tlsTermination
  type: boolean
- description: ''
  name: tags
  type: object
provider_name: Scalability
provider_slug: scalability
schema_file: json-schema/scalability-load-balancer-schema.json
slug: scalability-load-balancer
source_filename: scalability-load-balancer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalability/main/json-schema/scalability-load-balancer-schema.json\",\n  \"title\": \"Load Balancer\",\n  \"description\": \"Describes a load balancer configuration for distributing network traffic across multiple compute resources to ensure high availability and scalability.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\", \"backends\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the load balancer.\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the load balancer.\",\n      \"minLength\": 1\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Layer at which the load balancer operates.\",\n      \"enum\": [\"L4\", \"L7\", \"Global\", \"Regional\",\
  \ \"Application\", \"Network\", \"Gateway\"]\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"Traffic distribution algorithm.\",\n      \"enum\": [\"round-robin\", \"least-connections\", \"ip-hash\", \"weighted\", \"random\", \"resource-based\"],\n      \"default\": \"round-robin\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Network protocol.\",\n      \"enum\": [\"HTTP\", \"HTTPS\", \"TCP\", \"UDP\", \"gRPC\"],\n      \"default\": \"HTTPS\"\n    },\n    \"frontendPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Port on which the load balancer listens for incoming traffic.\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"healthCheck\": {\n      \"$ref\": \"#/$defs/HealthCheck\"\n    },\n    \"backends\": {\n      \"type\": \"array\",\n      \"description\": \"List of backend targets receiving distributed traffic.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\"\
  : \"#/$defs/Backend\"\n      }\n    },\n    \"stickySession\": {\n      \"type\": \"object\",\n      \"description\": \"Session affinity/persistence configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"cookieName\": {\n          \"type\": \"string\"\n        },\n        \"ttlSeconds\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"tlsTermination\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether TLS is terminated at the load balancer.\",\n      \"default\": false\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Backend\": {\n      \"type\": \"object\",\n      \"required\": [\"address\", \"port\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique\
  \ identifier for the backend.\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"IP address or hostname of the backend server.\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        },\n        \"weight\": {\n          \"type\": \"integer\",\n          \"description\": \"Relative weight for weighted load balancing.\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"default\": 1\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"healthy\", \"unhealthy\", \"draining\", \"unknown\"],\n          \"default\": \"unknown\"\n        }\n      }\n    },\n    \"HealthCheck\": {\n      \"type\": \"object\",\n      \"description\": \"Health check configuration for backend servers.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": true\n        },\n  \
  \      \"protocol\": {\n          \"type\": \"string\",\n          \"enum\": [\"HTTP\", \"HTTPS\", \"TCP\"],\n          \"default\": \"HTTP\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP path for health check requests.\",\n          \"default\": \"/health\"\n        },\n        \"intervalSeconds\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 30\n        },\n        \"timeoutSeconds\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 5\n        },\n        \"healthyThreshold\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 2\n        },\n        \"unhealthyThreshold\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 3\n        },\n        \"expectedStatusCodes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"integer\"\n          },\n   \
  \       \"default\": [200]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalability/refs/heads/main/json-schema/scalability-load-balancer-schema.json
tags:
- Auto Scaling
- Cloud Computing
- DevOps
- Distributed Systems
- Elasticity
- High Availability
- Infrastructure
- Load Balancing
- Performance
- Scalability
title: Load Balancer
---
