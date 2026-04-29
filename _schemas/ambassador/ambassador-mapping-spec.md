---
description: Specification for an Ambassador Mapping
layout: schema
name: MappingSpec
properties_list:
- description: Hostname to match for this Mapping. Use '*' to match all hostnames.
  name: hostname
  type: string
- description: URL prefix to match for routing
  name: prefix
  type: string
- description: Whether the prefix should be interpreted as a regular expression
  name: prefix_regex
  type: boolean
- description: Whether the prefix should be matched exactly rather than as a prefix
  name: prefix_exact
  type: boolean
- description: Target service to route to, in the format service-name.namespace:port or a full URL
  name: service
  type: string
- description: Prefix rewrite rule applied to the URL before forwarding to the backend service. Set to empty string to disable rewriting.
  name: rewrite
  type: string
- description: HTTP method to match
  name: method
  type: string
- description: Whether the method value is a regular expression
  name: method_regex
  type: boolean
- description: HTTP headers that must be present on the request for this Mapping to match. Values can be exact strings or regular expressions.
  name: headers
  type: object
- description: Query parameters that must be present for this Mapping to match
  name: query_parameters
  type: object
- description: Deprecated. Use hostname instead.
  name: host
  type: string
- description: Deprecated. Whether host is a regular expression.
  name: host_regex
  type: boolean
- description: Request timeout in milliseconds
  name: timeout_ms
  type: integer
- description: Idle timeout for streaming connections in milliseconds
  name: idle_timeout_ms
  type: integer
- description: Upstream connection timeout in milliseconds
  name: connect_timeout_ms
  type: integer
- description: Idle timeout for upstream connections in the cluster in milliseconds
  name: cluster_idle_timeout_ms
  type: integer
- description: Weight for traffic splitting when multiple Mappings match the same prefix. Used in canary deployments.
  name: weight
  type: integer
- description: Whether to bypass the external authentication service for this Mapping
  name: bypass_auth
  type: boolean
- description: Circuit breaker configurations for the upstream cluster
  name: circuit_breakers
  type: array
- description: Rate limiting labels to apply to requests matching this Mapping. Labels are sent to the rate limiting service for evaluation.
  name: labels
  type: object
- description: Headers to add to the request before forwarding to the upstream
  name: add_request_headers
  type: object
- description: Headers to add to the response before sending to the client
  name: add_response_headers
  type: object
- description: Header names to remove from the request
  name: remove_request_headers
  type: array
- description: Header names to remove from the response
  name: remove_response_headers
  type: array
- description: Protocols to allow upgrade to, such as websocket
  name: allow_upgrade
  type: array
- description: Whether the upstream service uses gRPC
  name: grpc
  type: boolean
- description: Whether to enable IPv4 DNS lookups for the upstream service
  name: enable_ipv4
  type: boolean
- description: Whether to enable IPv6 DNS lookups for the upstream service
  name: enable_ipv6
  type: boolean
- description: List of Ambassador IDs that should apply this Mapping. Used to partition a single Kubernetes cluster among multiple Ambassador instances.
  name: ambassador_id
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-mapping-spec-schema.json
slug: ambassador-mapping-spec
source_filename: ambassador-mapping-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for an Ambassador Mapping\",\n  \"properties\": {\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname to match for this Mapping. Use '*' to match all hostnames.\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"URL prefix to match for routing\"\n    },\n    \"prefix_regex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the prefix should be interpreted as a regular expression\"\n    },\n    \"prefix_exact\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the prefix should be matched exactly rather than as a prefix\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"Target service to route to, in the format service-name.namespace:port or a full URL\"\n    },\n    \"rewrite\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Prefix rewrite rule applied to the URL before forwarding to the backend service. Set to empty string to disable rewriting.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method to match\"\n    },\n    \"method_regex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the method value is a regular expression\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP headers that must be present on the request for this Mapping to match. Values can be exact strings or regular expressions.\"\n    },\n    \"query_parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Query parameters that must be present for this Mapping to match\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Deprecated. Use hostname instead.\"\n    },\n    \"host_regex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deprecated.\
  \ Whether host is a regular expression.\"\n    },\n    \"timeout_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Request timeout in milliseconds\"\n    },\n    \"idle_timeout_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Idle timeout for streaming connections in milliseconds\"\n    },\n    \"connect_timeout_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Upstream connection timeout in milliseconds\"\n    },\n    \"cluster_idle_timeout_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Idle timeout for upstream connections in the cluster in milliseconds\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight for traffic splitting when multiple Mappings match the same prefix. Used in canary deployments.\"\n    },\n    \"bypass_auth\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to bypass the external authentication service for this Mapping\"\n    },\n    \"circuit_breakers\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Circuit breaker configurations for the upstream cluster\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Rate limiting labels to apply to requests matching this Mapping. Labels are sent to the rate limiting service for evaluation.\"\n    },\n    \"add_request_headers\": {\n      \"type\": \"object\",\n      \"description\": \"Headers to add to the request before forwarding to the upstream\"\n    },\n    \"add_response_headers\": {\n      \"type\": \"object\",\n      \"description\": \"Headers to add to the response before sending to the client\"\n    },\n    \"remove_request_headers\": {\n      \"type\": \"array\",\n      \"description\": \"Header names to remove from the request\"\n    },\n    \"remove_response_headers\": {\n      \"type\": \"array\",\n      \"description\": \"Header names to remove from the response\"\n    },\n    \"allow_upgrade\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Protocols to allow upgrade to, such as websocket\"\n    },\n    \"grpc\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the upstream service uses gRPC\"\n    },\n    \"enable_ipv4\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable IPv4 DNS lookups for the upstream service\"\n    },\n    \"enable_ipv6\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable IPv6 DNS lookups for the upstream service\"\n    },\n    \"ambassador_id\": {\n      \"type\": \"array\",\n      \"description\": \"List of Ambassador IDs that should apply this Mapping. Used to partition a single Kubernetes cluster among multiple Ambassador instances.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-mapping-spec-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: MappingSpec
---
