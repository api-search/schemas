---
description: Schema for a load balancer configuration in a scalable distributed system.
layout: schema
name: Load Balancer Configuration
properties_list:
- description: Identifier for this load balancer.
  name: name
  type: string
- description: Load balancing algorithm for distributing traffic.
  name: algorithm
  type: string
- description: 'OSI layer: 4 = TCP/UDP, 7 = HTTP/HTTPS.'
  name: layer
  type: integer
- description: Virtual IP address or hostname for the load balancer frontend.
  name: virtualAddress
  type: string
- description: Listening port.
  name: port
  type: integer
- description: Protocol the load balancer handles.
  name: protocol
  type: string
- description: Session affinity configuration.
  name: stickySession
  type: object
- description: Health check configuration for backend servers.
  name: healthCheck
  type: object
- description: List of backend server instances.
  name: backends
  type: array
- description: TLS/SSL termination configuration.
  name: tlsTermination
  type: object
provider_name: Scalable Systems
provider_slug: scalable-systems
schema_file: json-schema/scalable-systems-load-balancer-schema.json
slug: scalable-systems-load-balancer
source_filename: scalable-systems-load-balancer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.com/schemas/scalable-systems/load-balancer\",\n  \"title\": \"Load Balancer Configuration\",\n  \"description\": \"Schema for a load balancer configuration in a scalable distributed system.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"algorithm\", \"backends\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for this load balancer.\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"enum\": [\"round-robin\", \"least-connections\", \"ip-hash\", \"weighted-round-robin\", \"random\", \"leasttime\"],\n      \"description\": \"Load balancing algorithm for distributing traffic.\"\n    },\n    \"layer\": {\n      \"type\": \"integer\",\n      \"enum\": [4, 7],\n      \"description\": \"OSI layer: 4 = TCP/UDP, 7 = HTTP/HTTPS.\"\n    },\n    \"virtualAddress\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Virtual IP address or hostname for the load balancer frontend.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"description\": \"Listening port.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\"http\", \"https\", \"tcp\", \"udp\", \"grpc\"],\n      \"description\": \"Protocol the load balancer handles.\"\n    },\n    \"stickySession\": {\n      \"type\": \"object\",\n      \"description\": \"Session affinity configuration.\",\n      \"properties\": {\n        \"enabled\": { \"type\": \"boolean\" },\n        \"cookieName\": {\n          \"type\": \"string\",\n          \"description\": \"Cookie name for sticky session routing.\"\n        },\n        \"ttlSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Session affinity duration in seconds.\"\n        }\n      }\n    },\n    \"healthCheck\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Health check configuration for backend servers.\",\n      \"required\": [\"path\", \"intervalSeconds\"],\n      \"properties\": {\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP path for health check.\",\n          \"example\": \"/healthz\"\n        },\n        \"intervalSeconds\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Seconds between health checks.\"\n        },\n        \"timeoutSeconds\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Seconds to wait for health check response.\"\n        },\n        \"healthyThreshold\": {\n          \"type\": \"integer\",\n          \"description\": \"Consecutive successes required to mark backend healthy.\"\n        },\n        \"unhealthyThreshold\": {\n          \"type\": \"integer\",\n          \"description\": \"Consecutive failures required to mark backend unhealthy.\"\n        }\n      }\n    },\n\
  \    \"backends\": {\n      \"type\": \"array\",\n      \"description\": \"List of backend server instances.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"address\", \"port\"],\n        \"properties\": {\n          \"address\": {\n            \"type\": \"string\",\n            \"description\": \"IP address or hostname of the backend.\"\n          },\n          \"port\": {\n            \"type\": \"integer\",\n            \"minimum\": 1,\n            \"maximum\": 65535\n          },\n          \"weight\": {\n            \"type\": \"integer\",\n            \"minimum\": 1,\n            \"maximum\": 100,\n            \"description\": \"Relative weight for weighted algorithms.\"\n          },\n          \"maxConnections\": {\n            \"type\": \"integer\",\n            \"description\": \"Maximum concurrent connections to this backend.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"default\"\
  : true\n          }\n        }\n      }\n    },\n    \"tlsTermination\": {\n      \"type\": \"object\",\n      \"description\": \"TLS/SSL termination configuration.\",\n      \"properties\": {\n        \"enabled\": { \"type\": \"boolean\" },\n        \"certificatePath\": { \"type\": \"string\" },\n        \"privateKeyPath\": { \"type\": \"string\" },\n        \"minimumTlsVersion\": {\n          \"type\": \"string\",\n          \"enum\": [\"1.2\", \"1.3\"],\n          \"default\": \"1.2\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-systems/refs/heads/main/json-schema/scalable-systems-load-balancer-schema.json
tags:
- Auto Scaling
- Caching
- Cloud Infrastructure
- Distributed Systems
- High Availability
- Infrastructure
- Load Balancing
- Message Queues
- Platform Engineering
- Scalable Architecture
- Service Discovery
title: Load Balancer Configuration
---
