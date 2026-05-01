---
description: A listener configuration defines a network address and port where Envoy accepts connections, along with filter chains that process those connections through a pipeline of network and HTTP filters.
layout: schema
name: Envoy Listener
properties_list:
- description: Unique name for the listener.
  name: name
  type: string
- description: The address the listener listens on for new connections.
  name: address
  type: object
- description: Filter chains to process connections received by the listener.
  name: filter_chains
  type: array
- description: Filters applied at the listener level before filter chain matching.
  name: listener_filters
  type: array
- description: Specifies the intended direction of traffic for the listener.
  name: traffic_direction
  type: string
- description: Soft limit on read and write buffer size per connection.
  name: per_connection_buffer_limit_bytes
  type: integer
- description: Whether the listener should bind to the port. Used for virtual listeners.
  name: bind_to_port
  type: boolean
- description: Whether to use SO_REUSEPORT for the listener socket.
  name: enable_reuse_port
  type: boolean
- description: The maximum length of the TCP pending connections queue.
  name: tcp_backlog_size
  type: integer
- description: Whether the listener should use transparent mode.
  name: transparent
  type: boolean
- description: Whether to set IP_FREEBIND socket option.
  name: freebind
  type: boolean
- description: Access log configuration for the listener.
  name: access_log
  type: array
- description: Balances connections across worker threads.
  name: connection_balance_config
  type: object
- description: Metadata for the listener.
  name: metadata
  type: object
provider_name: Envoy
provider_slug: envoy
schema_file: json-schema/envoy-listener.json
slug: envoy-listener
source_filename: envoy-listener.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.envoyproxy.io/schemas/listener\",\n  \"title\": \"Envoy Listener\",\n  \"description\": \"A listener configuration defines a network address and port where Envoy accepts connections, along with filter chains that process those connections through a pipeline of network and HTTP filters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the listener.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"The address the listener listens on for new connections.\",\n      \"properties\": {\n        \"socket_address\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"protocol\": {\n              \"type\": \"string\",\n              \"enum\": [\"TCP\", \"UDP\"],\n              \"default\": \"TCP\"\n            },\n            \"address\": {\n\
  \              \"type\": \"string\",\n              \"description\": \"IP address or hostname to bind to.\"\n            },\n            \"port_value\": {\n              \"type\": \"integer\",\n              \"description\": \"Port number to bind to.\",\n              \"minimum\": 0,\n              \"maximum\": 65535\n            }\n          },\n          \"required\": [\"address\", \"port_value\"]\n        },\n        \"pipe\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"path\": {\n              \"type\": \"string\",\n              \"description\": \"Unix domain socket path.\"\n            },\n            \"mode\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    },\n    \"filter_chains\": {\n      \"type\": \"array\",\n      \"description\": \"Filter chains to process connections received by the listener.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"filter_chain_match\"\
  : {\n            \"type\": \"object\",\n            \"description\": \"Match criteria for selecting this filter chain.\",\n            \"properties\": {\n              \"destination_port\": {\n                \"type\": \"integer\"\n              },\n              \"prefix_ranges\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"address_prefix\": { \"type\": \"string\" },\n                    \"prefix_len\": { \"type\": \"integer\" }\n                  }\n                }\n              },\n              \"server_names\": {\n                \"type\": \"array\",\n                \"description\": \"SNI domains to match.\",\n                \"items\": { \"type\": \"string\" }\n              },\n              \"transport_protocol\": {\n                \"type\": \"string\",\n                \"description\": \"Transport protocol to match (e.g., 'tls', 'raw_buffer').\"\n\
  \              },\n              \"application_protocols\": {\n                \"type\": \"array\",\n                \"description\": \"ALPN protocols to match.\",\n                \"items\": { \"type\": \"string\" }\n              }\n            }\n          },\n          \"filters\": {\n            \"type\": \"array\",\n            \"description\": \"Network filters in the chain.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Name of the filter (e.g., 'envoy.filters.network.http_connection_manager').\"\n                },\n                \"typed_config\": {\n                  \"type\": \"object\",\n                  \"description\": \"Filter-specific typed configuration.\"\n                }\n              },\n              \"required\": [\"name\"]\n            }\n          },\n          \"transport_socket\": {\n            \"\
  type\": \"object\",\n            \"description\": \"Transport socket for this filter chain (e.g., TLS).\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"typed_config\": {\n                \"type\": \"object\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"listener_filters\": {\n      \"type\": \"array\",\n      \"description\": \"Filters applied at the listener level before filter chain matching.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the listener filter (e.g., 'envoy.filters.listener.tls_inspector').\"\n          },\n          \"typed_config\": {\n            \"type\": \"object\"\n          }\n        },\n        \"required\": [\"name\"]\n      }\n    },\n    \"traffic_direction\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Specifies the intended direction of traffic for the listener.\",\n      \"enum\": [\"UNSPECIFIED\", \"INBOUND\", \"OUTBOUND\"]\n    },\n    \"per_connection_buffer_limit_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Soft limit on read and write buffer size per connection.\"\n    },\n    \"bind_to_port\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the listener should bind to the port. Used for virtual listeners.\",\n      \"default\": true\n    },\n    \"enable_reuse_port\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use SO_REUSEPORT for the listener socket.\"\n    },\n    \"tcp_backlog_size\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum length of the TCP pending connections queue.\"\n    },\n    \"transparent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the listener should use transparent mode.\"\n    },\n    \"freebind\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether to set IP_FREEBIND socket option.\"\n    },\n    \"access_log\": {\n      \"type\": \"array\",\n      \"description\": \"Access log configuration for the listener.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"typed_config\": {\n            \"type\": \"object\"\n          },\n          \"filter\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"connection_balance_config\": {\n      \"type\": \"object\",\n      \"description\": \"Balances connections across worker threads.\",\n      \"properties\": {\n        \"exact_balance\": {\n          \"type\": \"object\"\n        }\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for the listener.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"name\", \"address\", \"filter_chains\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/json-schema/envoy-listener.json
tags:
- Cloud Native
- Load Balancing
- Proxy
- Service Mesh
title: Envoy Listener
---
