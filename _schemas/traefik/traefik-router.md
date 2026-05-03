---
description: Represents an HTTP, TCP, or UDP router in a running Traefik instance, including its routing rule, entry points, service assignment, and middleware chain.
layout: schema
name: Traefik Router
properties_list:
- description: The name of the router in name@provider format.
  name: name
  type: string
- description: Entry points this router is bound to.
  name: entryPoints
  type: array
- description: The routing rule expression used to match incoming requests (e.g., Host, Path, Headers matchers for HTTP; HostSNI for TCP).
  name: rule
  type: string
- description: The syntax version of the rule expression.
  name: ruleSyntax
  type: string
- description: The priority of the router when multiple routers match the same request. Higher values take precedence.
  name: priority
  type: integer
- description: The name of the service this router routes traffic to.
  name: service
  type: string
- description: Ordered list of middleware names applied to requests handled by this router.
  name: middlewares
  type: array
- description: The current operational status of the router.
  name: status
  type: string
- description: The configuration provider that created this router (e.g., docker, kubernetes, file).
  name: provider
  type: string
- description: The protocol this router handles.
  name: protocol
  type: string
- description: TLS configuration for this router, if TLS termination is enabled.
  name: tls
  type: object
- description: Entry points currently being used by this router.
  name: using
  type: array
provider_name: Traefik
provider_slug: traefik
schema_file: json-schema/traefik-router-schema.json
slug: traefik-router
source_filename: traefik-router-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://traefik.io/schemas/traefik/router.json\",\n  \"title\": \"Traefik Router\",\n  \"description\": \"Represents an HTTP, TCP, or UDP router in a running Traefik instance, including its routing rule, entry points, service assignment, and middleware chain.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the router in name@provider format.\",\n      \"minLength\": 1\n    },\n    \"entryPoints\": {\n      \"type\": \"array\",\n      \"description\": \"Entry points this router is bound to.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"rule\": {\n      \"type\": \"string\",\n      \"description\": \"The routing rule expression used to match incoming requests (e.g., Host, Path, Headers matchers for HTTP; HostSNI for TCP).\"\n    },\n    \"ruleSyntax\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"The syntax version of the rule expression.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority of the router when multiple routers match the same request. Higher values take precedence.\",\n      \"minimum\": 0\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service this router routes traffic to.\"\n    },\n    \"middlewares\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of middleware names applied to requests handled by this router.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current operational status of the router.\",\n      \"enum\": [\"enabled\", \"disabled\", \"warning\"]\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The configuration provider that created this\
  \ router (e.g., docker, kubernetes, file).\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol this router handles.\",\n      \"enum\": [\"http\", \"tcp\", \"udp\"]\n    },\n    \"tls\": {\n      \"$ref\": \"#/$defs/TLSConfig\",\n      \"description\": \"TLS configuration for this router, if TLS termination is enabled.\"\n    },\n    \"using\": {\n      \"type\": \"array\",\n      \"description\": \"Entry points currently being used by this router.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"TLSConfig\": {\n      \"type\": \"object\",\n      \"description\": \"TLS configuration for a router, including certificate resolver and domain settings.\",\n      \"properties\": {\n        \"passthrough\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether TLS connections are passed through to the backend without termination (TCP only).\"\n        },\n        \"options\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Name of the TLS options configuration to use.\"\n        },\n        \"certResolver\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the certificate resolver to use for automatic TLS certificate provisioning.\"\n        },\n        \"domains\": {\n          \"type\": \"array\",\n          \"description\": \"Domain configurations for certificate generation.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Domain\"\n          }\n        }\n      }\n    },\n    \"Domain\": {\n      \"type\": \"object\",\n      \"description\": \"Domain configuration for TLS certificate generation.\",\n      \"properties\": {\n        \"main\": {\n          \"type\": \"string\",\n          \"description\": \"The main domain name for the certificate.\"\n        },\n        \"sans\": {\n          \"type\": \"array\",\n          \"description\": \"Subject Alternative Names for the certificate.\",\n          \"\
  items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traefik/refs/heads/main/json-schema/traefik-router-schema.json
tags:
- API Gateway
- Kubernetes
- Load Balancer
- Open Source
- Reverse Proxy
title: Traefik Router
---
