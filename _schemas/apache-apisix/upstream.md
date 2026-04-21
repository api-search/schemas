---
description: An Upstream is a virtual host abstraction that performs load balancing on a given set of service nodes according to configured rules.
layout: schema
name: Apache APISIX Upstream
properties_list:
- description: Human-readable name for the upstream.
  name: name
  type: string
- description: Description of the upstream.
  name: desc
  type: string
- description: Load balancing algorithm.
  name: type
  type: string
- description: Backend service nodes.
  name: nodes
  type: object
- description: Service name for service discovery.
  name: service_name
  type: string
- description: Type of service discovery (e.g. dns, consul, nacos, eureka).
  name: discovery_type
  type: string
- description: Hash input for consistent hashing load balancer.
  name: hash_on
  type: string
- description: Hash key when using chash load balancer.
  name: key
  type: string
- description: Health check configuration.
  name: checks
  type: object
- description: Number of retries for failed requests.
  name: retries
  type: integer
- description: Timeout in seconds for retry requests.
  name: retry_timeout
  type: number
- description: Timeout settings for upstream connections.
  name: timeout
  type: object
- description: The scheme for communicating with the upstream.
  name: scheme
  type: string
- description: How to set the Host header when proxying to upstream.
  name: pass_host
  type: string
- description: Host to use when pass_host is set to rewrite.
  name: upstream_host
  type: string
- description: Key-value pairs for categorization.
  name: labels
  type: object
- description: Keepalive pool configuration.
  name: keepalive_pool
  type: object
- description: TLS configuration for upstream connections.
  name: tls
  type: object
provider_name: Apache APISIX
provider_slug: apache-apisix
schema_file: json-schema/upstream.json
slug: upstream
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
title: Apache APISIX Upstream
---
