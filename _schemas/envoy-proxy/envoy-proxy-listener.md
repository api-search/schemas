---
description: An Envoy Proxy Listener defines a network address and port where Envoy accepts downstream connections. Each listener specifies one or more filter chains that process incoming traffic, allowing Envoy to route, transform, and manage connections. Listeners support both TCP and UDP protocols and can be configured with TLS termination, connection limits, and traffic mirroring.
layout: schema
name: Envoy Proxy Listener
properties_list:
- description: The unique name for this listener, used in statistics and logging.
  name: name
  type: string
- description: The address and port that the listener should bind to.
  name: address
  type: object
- description: A list of filter chains to process connections received by this listener. Each filter chain contains a series of network filters.
  name: filter_chains
  type: array
- description: Listener filters that are applied before the filter chain is selected.
  name: listener_filters
  type: array
- description: Soft limit on size of the listener's new connection read and write buffers in bytes.
  name: per_connection_buffer_limit_bytes
  type: integer
- description: Specifies the intended direction of the traffic relative to the local Envoy.
  name: traffic_direction
  type: string
- description: Whether the listener should use SO_REUSEPORT for binding.
  name: enable_reuse_port
  type: boolean
- description: Configuration for access logging on this listener.
  name: access_log
  type: array
provider_name: Envoy Proxy
provider_slug: envoy-proxy
schema_file: json-schema/envoy-proxy-listener.json
slug: envoy-proxy-listener
source_filename: envoy-proxy-listener.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"envoy-proxy-listener.json\",\n  \"title\": \"Envoy Proxy Listener\",\n  \"description\": \"An Envoy Proxy Listener defines a network address and port where Envoy accepts downstream connections. Each listener specifies one or more filter chains that process incoming traffic, allowing Envoy to route, transform, and manage connections. Listeners support both TCP and UDP protocols and can be configured with TLS termination, connection limits, and traffic mirroring.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name for this listener, used in statistics and logging.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"The address and port that the listener should bind to.\",\n      \"properties\": {\n        \"socket_address\": {\n          \"type\": \"object\",\n          \"description\"\
  : \"A TCP or UDP socket address.\",\n          \"properties\": {\n            \"address\": {\n              \"type\": \"string\",\n              \"description\": \"The IP address or hostname to bind to. Use 0.0.0.0 for all interfaces.\"\n            },\n            \"port_value\": {\n              \"type\": \"integer\",\n              \"description\": \"The port number to bind to.\",\n              \"minimum\": 0,\n              \"maximum\": 65535\n            },\n            \"protocol\": {\n              \"type\": \"string\",\n              \"description\": \"The protocol to use for the socket.\",\n              \"enum\": [\"TCP\", \"UDP\"]\n            }\n          },\n          \"required\": [\"address\", \"port_value\"]\n        }\n      }\n    },\n    \"filter_chains\": {\n      \"type\": \"array\",\n      \"description\": \"A list of filter chains to process connections received by this listener. Each filter chain contains a series of network filters.\",\n      \"items\": {\n  \
  \      \"type\": \"object\",\n        \"properties\": {\n          \"filter_chain_match\": {\n            \"type\": \"object\",\n            \"description\": \"Criteria for matching a connection to this filter chain.\",\n            \"properties\": {\n              \"destination_port\": {\n                \"type\": \"integer\",\n                \"description\": \"The destination port to match.\"\n              },\n              \"server_names\": {\n                \"type\": \"array\",\n                \"description\": \"SNI server names to match for TLS connections.\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"transport_protocol\": {\n                \"type\": \"string\",\n                \"description\": \"The transport protocol to match, such as tls or raw_buffer.\"\n              },\n              \"application_protocols\": {\n                \"type\": \"array\",\n                \"description\": \"ALPN\
  \ protocols to match.\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"The ordered list of network filters that make up this filter chain.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"The name of the filter, such as envoy.filters.network.http_connection_manager.\"\n                },\n                \"typed_config\": {\n                  \"type\": \"object\",\n                  \"description\": \"The typed configuration for this filter.\",\n                  \"additionalProperties\": true\n                }\n              },\n              \"required\": [\"name\"]\n            }\n          },\n          \"transport_socket\": {\n            \"type\"\
  : \"object\",\n            \"description\": \"Optional transport socket configuration, typically for TLS.\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The transport socket name, typically envoy.transport_sockets.tls.\"\n              },\n              \"typed_config\": {\n                \"type\": \"object\",\n                \"description\": \"The typed TLS configuration.\",\n                \"additionalProperties\": true\n              }\n            }\n          }\n        }\n      }\n    },\n    \"listener_filters\": {\n      \"type\": \"array\",\n      \"description\": \"Listener filters that are applied before the filter chain is selected.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the listener filter.\"\n          },\n          \"typed_config\": {\n  \
  \          \"type\": \"object\",\n            \"description\": \"The typed configuration for this listener filter.\",\n            \"additionalProperties\": true\n          }\n        },\n        \"required\": [\"name\"]\n      }\n    },\n    \"per_connection_buffer_limit_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Soft limit on size of the listener's new connection read and write buffers in bytes.\"\n    },\n    \"traffic_direction\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the intended direction of the traffic relative to the local Envoy.\",\n      \"enum\": [\"UNSPECIFIED\", \"INBOUND\", \"OUTBOUND\"]\n    },\n    \"enable_reuse_port\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the listener should use SO_REUSEPORT for binding.\"\n    },\n    \"access_log\": {\n      \"type\": \"array\",\n      \"description\": \"Configuration for access logging on this listener.\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the access log implementation.\"\n          },\n          \"typed_config\": {\n            \"type\": \"object\",\n            \"description\": \"The typed configuration for the access log.\",\n            \"additionalProperties\": true\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"address\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/envoy-proxy/refs/heads/main/json-schema/envoy-proxy-listener.json
tags:
- Gateways
- Proxies
title: Envoy Proxy Listener
---
