---
description: Represents an HTTP, TCP, or UDP service in a running Traefik instance, including its load balancer configuration, backend servers, and health check settings.
layout: schema
name: Traefik Service
properties_list:
- description: The name of the service in name@provider format.
  name: name
  type: string
- description: The type of service.
  name: type
  type: string
- description: The current operational status of the service.
  name: status
  type: string
- description: The configuration provider that created this service (e.g., docker, kubernetes, file).
  name: provider
  type: string
- description: The protocol this service handles.
  name: protocol
  type: string
- description: Load balancer configuration including backend servers and health checks.
  name: loadBalancer
  type: object
- description: Map of server URLs to their current health status.
  name: serverStatus
  type: object
provider_name: Traefik
provider_slug: traefik
schema_file: json-schema/traefik-service-schema.json
slug: traefik-service
source_filename: traefik-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://traefik.io/schemas/traefik/service.json\",\n  \"title\": \"Traefik Service\",\n  \"description\": \"Represents an HTTP, TCP, or UDP service in a running Traefik instance, including its load balancer configuration, backend servers, and health check settings.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service in name@provider format.\",\n      \"minLength\": 1\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of service.\",\n      \"enum\": [\"loadBalancer\", \"weighted\", \"mirroring\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current operational status of the service.\",\n      \"enum\": [\"enabled\", \"disabled\", \"warning\"]\n    },\n    \"provider\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The configuration provider that created this service (e.g., docker, kubernetes, file).\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol this service handles.\",\n      \"enum\": [\"http\", \"tcp\", \"udp\"]\n    },\n    \"loadBalancer\": {\n      \"$ref\": \"#/$defs/LoadBalancer\",\n      \"description\": \"Load balancer configuration including backend servers and health checks.\"\n    },\n    \"serverStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Map of server URLs to their current health status.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"LoadBalancer\": {\n      \"type\": \"object\",\n      \"description\": \"Load balancer configuration distributing traffic across backend servers.\",\n      \"properties\": {\n        \"servers\": {\n          \"type\": \"array\",\n          \"description\": \"List of backend servers to\
  \ load balance across.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Server\"\n          }\n        },\n        \"passHostHeader\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to pass the original Host header to backend servers.\"\n        },\n        \"healthCheck\": {\n          \"$ref\": \"#/$defs/HealthCheck\",\n          \"description\": \"Health check configuration for monitoring backend server availability.\"\n        }\n      }\n    },\n    \"Server\": {\n      \"type\": \"object\",\n      \"description\": \"A backend server in the load balancer pool.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the backend server (HTTP/HTTPS services).\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"The address of the backend server in host:port format (TCP/UDP services).\"\n        }\n    \
  \  }\n    },\n    \"HealthCheck\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for periodic health checks against backend servers.\",\n      \"properties\": {\n        \"scheme\": {\n          \"type\": \"string\",\n          \"description\": \"The scheme to use for health check requests (http or https).\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"The path to use for health check requests.\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port to use for health check requests.\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        },\n        \"interval\": {\n          \"type\": \"string\",\n          \"description\": \"The interval between health checks (e.g., '10s', '30s').\"\n        },\n        \"timeout\": {\n          \"type\": \"string\",\n          \"description\": \"The timeout for each health check request (e.g., '5s').\"\n      \
  \  }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/json-schema/traefik-service-schema.json
tags:
- API Gateway
- Kubernetes
- Load Balancer
- Open Source
- Reverse Proxy
title: Traefik Service
---
