---
description: An upstream cluster represents a group of logically similar upstream hosts that Envoy connects to. Clusters define how Envoy discovers, health checks, load balances, and connects to upstream services.
layout: schema
name: Envoy Cluster
properties_list:
- description: Unique name for the cluster, used to reference it in route configurations and stats.
  name: name
  type: string
- description: The service discovery type to use for resolving cluster member endpoints.
  name: type
  type: string
- description: Timeout for new network connections to upstream hosts (e.g., '5s').
  name: connect_timeout
  type: string
- description: The load balancing algorithm used to select an upstream host.
  name: lb_policy
  type: string
- description: Endpoint assignment for STATIC and EDS clusters.
  name: load_assignment
  type: object
- description: Configuration for using EDS to discover cluster members.
  name: eds_cluster_config
  type: object
- description: Health checking configuration for cluster members.
  name: health_checks
  type: array
- description: Circuit breaking limits for the cluster.
  name: circuit_breakers
  type: object
- description: Outlier detection configuration for ejecting unhealthy hosts.
  name: outlier_detection
  type: object
- description: Transport socket configuration for upstream connections (e.g., TLS).
  name: transport_socket
  type: object
- description: DNS IP address resolution policy for STRICT_DNS and LOGICAL_DNS clusters.
  name: dns_lookup_family
  type: string
- description: Custom DNS resolvers for the cluster.
  name: dns_resolvers
  type: array
- description: Whether to respect DNS TTL values for DNS-based clusters.
  name: respect_dns_ttl
  type: boolean
- description: DNS refresh rate for DNS-based clusters.
  name: dns_refresh_rate
  type: string
- description: Soft limit on size of the cluster's connections read and write buffers.
  name: per_connection_buffer_limit_bytes
  type: integer
- description: Metadata for the cluster, used for stats, logging, and access control.
  name: metadata
  type: object
- description: Common configuration shared by all load balancer implementations.
  name: common_lb_config
  type: object
provider_name: Envoy
provider_slug: envoy
schema_file: json-schema/envoy-cluster.json
slug: envoy-cluster
source_filename: envoy-cluster.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.envoyproxy.io/schemas/cluster\",\n  \"title\": \"Envoy Cluster\",\n  \"description\": \"An upstream cluster represents a group of logically similar upstream hosts that Envoy connects to. Clusters define how Envoy discovers, health checks, load balances, and connects to upstream services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the cluster, used to reference it in route configurations and stats.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The service discovery type to use for resolving cluster member endpoints.\",\n      \"enum\": [\"STATIC\", \"STRICT_DNS\", \"LOGICAL_DNS\", \"EDS\", \"ORIGINAL_DST\"]\n    },\n    \"connect_timeout\": {\n      \"type\": \"string\",\n      \"description\": \"Timeout for new network connections to upstream hosts (e.g.,\
  \ '5s').\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?s$\"\n    },\n    \"lb_policy\": {\n      \"type\": \"string\",\n      \"description\": \"The load balancing algorithm used to select an upstream host.\",\n      \"enum\": [\"ROUND_ROBIN\", \"LEAST_REQUEST\", \"RING_HASH\", \"RANDOM\", \"MAGLEV\", \"CLUSTER_PROVIDED\"]\n    },\n    \"load_assignment\": {\n      \"type\": \"object\",\n      \"description\": \"Endpoint assignment for STATIC and EDS clusters.\",\n      \"properties\": {\n        \"cluster_name\": {\n          \"type\": \"string\"\n        },\n        \"endpoints\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"locality\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"region\": { \"type\": \"string\" },\n                  \"zone\": { \"type\": \"string\" },\n                  \"sub_zone\": { \"type\": \"string\" }\n         \
  \       }\n              },\n              \"lb_endpoints\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"endpoint\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"address\": {\n                          \"type\": \"object\",\n                          \"properties\": {\n                            \"socket_address\": {\n                              \"type\": \"object\",\n                              \"properties\": {\n                                \"address\": { \"type\": \"string\" },\n                                \"port_value\": {\n                                  \"type\": \"integer\",\n                                  \"minimum\": 0,\n                                  \"maximum\": 65535\n                                }\n                              },\n                        \
  \      \"required\": [\"address\", \"port_value\"]\n                            }\n                          }\n                        }\n                      }\n                    },\n                    \"health_status\": {\n                      \"type\": \"string\",\n                      \"enum\": [\"UNKNOWN\", \"HEALTHY\", \"UNHEALTHY\", \"DRAINING\", \"TIMEOUT\", \"DEGRADED\"]\n                    },\n                    \"load_balancing_weight\": {\n                      \"type\": \"integer\",\n                      \"minimum\": 1\n                    }\n                  }\n                }\n              },\n              \"priority\": {\n                \"type\": \"integer\",\n                \"minimum\": 0\n              }\n            }\n          }\n        }\n      }\n    },\n    \"eds_cluster_config\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for using EDS to discover cluster members.\",\n      \"properties\": {\n        \"eds_config\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"api_config_source\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"api_type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"REST\", \"GRPC\", \"DELTA_GRPC\"]\n                },\n                \"grpc_services\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"cluster_names\": {\n                  \"type\": \"array\",\n                  \"items\": { \"type\": \"string\" }\n                }\n              }\n            },\n            \"ads\": { \"type\": \"object\" },\n            \"path\": { \"type\": \"string\" },\n            \"resource_api_version\": {\n              \"type\": \"string\",\n              \"enum\": [\"AUTO\", \"V2\", \"V3\"]\n            }\n          }\n        },\n        \"service_name\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Alternative service name used to look up endpoints via EDS.\"\n        }\n      }\n    },\n    \"health_checks\": {\n      \"type\": \"array\",\n      \"description\": \"Health checking configuration for cluster members.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timeout\": { \"type\": \"string\" },\n          \"interval\": { \"type\": \"string\" },\n          \"unhealthy_threshold\": { \"type\": \"integer\" },\n          \"healthy_threshold\": { \"type\": \"integer\" },\n          \"http_health_check\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"host\": { \"type\": \"string\" },\n              \"path\": { \"type\": \"string\" },\n              \"expected_statuses\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n              \
  \      \"start\": { \"type\": \"integer\" },\n                    \"end\": { \"type\": \"integer\" }\n                  }\n                }\n              }\n            }\n          },\n          \"tcp_health_check\": { \"type\": \"object\" },\n          \"grpc_health_check\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"service_name\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"circuit_breakers\": {\n      \"type\": \"object\",\n      \"description\": \"Circuit breaking limits for the cluster.\",\n      \"properties\": {\n        \"thresholds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"priority\": {\n                \"type\": \"string\",\n                \"enum\": [\"DEFAULT\", \"HIGH\"]\n              },\n              \"max_connections\": { \"type\": \"integer\" },\n              \"max_pending_requests\"\
  : { \"type\": \"integer\" },\n              \"max_requests\": { \"type\": \"integer\" },\n              \"max_retries\": { \"type\": \"integer\" },\n              \"track_remaining\": { \"type\": \"boolean\" }\n            }\n          }\n        }\n      }\n    },\n    \"outlier_detection\": {\n      \"type\": \"object\",\n      \"description\": \"Outlier detection configuration for ejecting unhealthy hosts.\",\n      \"properties\": {\n        \"consecutive_5xx\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of consecutive 5xx responses before ejection.\"\n        },\n        \"consecutive_gateway_failure\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of consecutive gateway failures before ejection.\"\n        },\n        \"interval\": {\n          \"type\": \"string\",\n          \"description\": \"Time interval between ejection analysis sweeps.\"\n        },\n        \"base_ejection_time\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Base time for which a host is ejected.\"\n        },\n        \"max_ejection_percent\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum percentage of hosts in the cluster that can be ejected.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"enforcing_consecutive_5xx\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"enforcing_success_rate\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"success_rate_minimum_hosts\": {\n          \"type\": \"integer\"\n        },\n        \"success_rate_request_volume\": {\n          \"type\": \"integer\"\n        },\n        \"success_rate_stdev_factor\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"transport_socket\": {\n      \"type\": \"object\",\n      \"description\": \"Transport socket configuration for\
  \ upstream connections (e.g., TLS).\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the transport socket implementation.\"\n        },\n        \"typed_config\": {\n          \"type\": \"object\",\n          \"description\": \"Transport socket specific configuration.\"\n        }\n      }\n    },\n    \"dns_lookup_family\": {\n      \"type\": \"string\",\n      \"description\": \"DNS IP address resolution policy for STRICT_DNS and LOGICAL_DNS clusters.\",\n      \"enum\": [\"AUTO\", \"V4_ONLY\", \"V6_ONLY\", \"V4_PREFERRED\", \"ALL\"]\n    },\n    \"dns_resolvers\": {\n      \"type\": \"array\",\n      \"description\": \"Custom DNS resolvers for the cluster.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"socket_address\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"address\": { \"type\": \"string\" },\n              \"port_value\"\
  : { \"type\": \"integer\" }\n            }\n          }\n        }\n      }\n    },\n    \"respect_dns_ttl\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to respect DNS TTL values for DNS-based clusters.\"\n    },\n    \"dns_refresh_rate\": {\n      \"type\": \"string\",\n      \"description\": \"DNS refresh rate for DNS-based clusters.\"\n    },\n    \"per_connection_buffer_limit_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Soft limit on size of the cluster's connections read and write buffers.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for the cluster, used for stats, logging, and access control.\",\n      \"additionalProperties\": true\n    },\n    \"common_lb_config\": {\n      \"type\": \"object\",\n      \"description\": \"Common configuration shared by all load balancer implementations.\",\n      \"properties\": {\n        \"healthy_panic_threshold\": {\n          \"type\": \"object\"\
  ,\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\",\n              \"minimum\": 0,\n              \"maximum\": 100\n            }\n          }\n        },\n        \"locality_weighted_lb_config\": {\n          \"type\": \"object\"\n        },\n        \"zone_aware_lb_config\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"routing_enabled\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": { \"type\": \"number\" }\n              }\n            },\n            \"min_cluster_size\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/envoy/refs/heads/main/json-schema/envoy-cluster.json
tags:
- Cloud Native
- Load Balancing
- Proxy
- Service Mesh
title: Envoy Cluster
---
