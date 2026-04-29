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
source_filename: upstream.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/apache-apisix/blob/main/json-schema/upstream.json\",\n  \"title\": \"Apache APISIX Upstream\",\n  \"description\": \"An Upstream is a virtual host abstraction that performs load balancing on a given set of service nodes according to configured rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the upstream.\"\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the upstream.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"roundrobin\", \"chash\", \"least_conn\", \"ewma\"],\n      \"default\": \"roundrobin\",\n      \"description\": \"Load balancing algorithm.\"\n    },\n    \"nodes\": {\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n  \
  \          \"type\": \"integer\"\n          },\n          \"description\": \"Key-value pairs of address:port to weight.\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"host\": {\n                \"type\": \"string\"\n              },\n              \"port\": {\n                \"type\": \"integer\"\n              },\n              \"weight\": {\n                \"type\": \"integer\"\n              },\n              \"priority\": {\n                \"type\": \"integer\",\n                \"default\": 0\n              }\n            }\n          },\n          \"description\": \"List of node objects.\"\n        }\n      ],\n      \"description\": \"Backend service nodes.\"\n    },\n    \"service_name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name for service discovery.\"\n    },\n    \"discovery_type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Type of service discovery (e.g. dns, consul, nacos, eureka).\"\n    },\n    \"hash_on\": {\n      \"type\": \"string\",\n      \"enum\": [\"vars\", \"header\", \"cookie\", \"consumer\", \"vars_combinations\"],\n      \"default\": \"vars\",\n      \"description\": \"Hash input for consistent hashing load balancer.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Hash key when using chash load balancer.\"\n    },\n    \"checks\": {\n      \"type\": \"object\",\n      \"description\": \"Health check configuration.\",\n      \"properties\": {\n        \"active\": {\n          \"type\": \"object\",\n          \"description\": \"Active health check configuration.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"http\", \"https\", \"tcp\"],\n              \"default\": \"http\"\n            },\n            \"timeout\": {\n              \"type\": \"number\",\n              \"default\": 1\n\
  \            },\n            \"http_path\": {\n              \"type\": \"string\",\n              \"default\": \"/\"\n            },\n            \"host\": {\n              \"type\": \"string\"\n            },\n            \"port\": {\n              \"type\": \"integer\"\n            },\n            \"https_verify_certificate\": {\n              \"type\": \"boolean\",\n              \"default\": true\n            },\n            \"healthy\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"interval\": {\n                  \"type\": \"integer\"\n                },\n                \"successes\": {\n                  \"type\": \"integer\"\n                }\n              }\n            },\n            \"unhealthy\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"interval\": {\n                  \"type\": \"integer\"\n                },\n                \"http_failures\": {\n                  \"type\":\
  \ \"integer\"\n                },\n                \"tcp_failures\": {\n                  \"type\": \"integer\"\n                },\n                \"timeouts\": {\n                  \"type\": \"integer\"\n                }\n              }\n            }\n          }\n        },\n        \"passive\": {\n          \"type\": \"object\",\n          \"description\": \"Passive health check configuration.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"http\", \"https\", \"tcp\"],\n              \"default\": \"http\"\n            },\n            \"healthy\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"http_statuses\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"integer\"\n                  }\n                },\n                \"successes\": {\n                  \"type\": \"integer\"\n                }\n   \
  \           }\n            },\n            \"unhealthy\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"http_statuses\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"integer\"\n                  }\n                },\n                \"http_failures\": {\n                  \"type\": \"integer\"\n                },\n                \"tcp_failures\": {\n                  \"type\": \"integer\"\n                },\n                \"timeouts\": {\n                  \"type\": \"integer\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"retries\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of retries for failed requests.\"\n    },\n    \"retry_timeout\": {\n      \"type\": \"number\",\n      \"description\": \"Timeout in seconds for retry requests.\"\n    },\n    \"timeout\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Timeout settings for upstream connections.\",\n      \"properties\": {\n        \"connect\": {\n          \"type\": \"number\",\n          \"default\": 60,\n          \"description\": \"Connection timeout in seconds.\"\n        },\n        \"send\": {\n          \"type\": \"number\",\n          \"default\": 60,\n          \"description\": \"Send timeout in seconds.\"\n        },\n        \"read\": {\n          \"type\": \"number\",\n          \"default\": 60,\n          \"description\": \"Read timeout in seconds.\"\n        }\n      }\n    },\n    \"scheme\": {\n      \"type\": \"string\",\n      \"enum\": [\"http\", \"https\", \"grpc\", \"grpcs\"],\n      \"default\": \"http\",\n      \"description\": \"The scheme for communicating with the upstream.\"\n    },\n    \"pass_host\": {\n      \"type\": \"string\",\n      \"enum\": [\"pass\", \"node\", \"rewrite\"],\n      \"default\": \"pass\",\n      \"description\": \"How to set the Host header when proxying to upstream.\"\
  \n    },\n    \"upstream_host\": {\n      \"type\": \"string\",\n      \"description\": \"Host to use when pass_host is set to rewrite.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for categorization.\"\n    },\n    \"keepalive_pool\": {\n      \"type\": \"object\",\n      \"description\": \"Keepalive pool configuration.\",\n      \"properties\": {\n        \"size\": {\n          \"type\": \"integer\",\n          \"default\": 320\n        },\n        \"idle_timeout\": {\n          \"type\": \"number\",\n          \"default\": 60\n        },\n        \"requests\": {\n          \"type\": \"integer\",\n          \"default\": 1000\n        }\n      }\n    },\n    \"tls\": {\n      \"type\": \"object\",\n      \"description\": \"TLS configuration for upstream connections.\",\n      \"properties\": {\n        \"client_cert\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"Client certificate for mTLS.\"\n        },\n        \"client_key\": {\n          \"type\": \"string\",\n          \"description\": \"Client private key for mTLS.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/json-schema/upstream.json
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
