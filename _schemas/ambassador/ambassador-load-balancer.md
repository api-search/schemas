---
description: Load balancing configuration for an upstream cluster
layout: schema
name: LoadBalancer
properties_list:
- description: Load balancing algorithm
  name: policy
  type: string
- description: Cookie-based session affinity configuration (for ring_hash policy)
  name: cookie
  type: object
- description: Header to use for hash-based load balancing
  name: header
  type: string
- description: Whether to use source IP for hash-based load balancing
  name: source_ip
  type: boolean
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-load-balancer-schema.json
slug: ambassador-load-balancer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoadBalancer\",\n  \"type\": \"object\",\n  \"description\": \"Load balancing configuration for an upstream cluster\",\n  \"properties\": {\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"Load balancing algorithm\"\n    },\n    \"cookie\": {\n      \"type\": \"object\",\n      \"description\": \"Cookie-based session affinity configuration (for ring_hash policy)\"\n    },\n    \"header\": {\n      \"type\": \"string\",\n      \"description\": \"Header to use for hash-based load balancing\"\n    },\n    \"source_ip\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use source IP for hash-based load balancing\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-load-balancer-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: LoadBalancer
---
