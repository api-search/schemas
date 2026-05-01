---
description: JSON Schema representing the Go Micro service configuration options including server, client, registry, broker, transport, and runtime settings.
layout: schema
name: Go Micro Service Options
properties_list:
- description: Server configuration options.
  name: server
  type: object
- description: Client configuration options.
  name: client
  type: object
- description: Service registry configuration.
  name: registry
  type: object
- description: Message broker configuration.
  name: broker
  type: object
- description: Transport layer configuration.
  name: transport
  type: object
- description: Service selector / load balancer configuration.
  name: selector
  type: object
- description: Runtime configuration.
  name: runtime
  type: object
provider_name: Go Micro
provider_slug: go-micro
schema_file: json-schema/go-micro-options.json
slug: go-micro-options
source_filename: go-micro-options.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/go-micro/json-schema/go-micro-options.json\",\n  \"title\": \"Go Micro Service Options\",\n  \"description\": \"JSON Schema representing the Go Micro service configuration options including server, client, registry, broker, transport, and runtime settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"server\": {\n      \"type\": \"object\",\n      \"description\": \"Server configuration options.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Service name.\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Bind address (host:port).\",\n          \"default\": \":0\"\n        },\n        \"advertise\": {\n          \"type\": \"string\",\n          \"description\": \"Address to advertise to the registry.\"\n        },\n        \"id\": {\n \
  \         \"type\": \"string\",\n          \"description\": \"Unique server ID.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Service version.\",\n          \"default\": \"latest\"\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Server metadata.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"registerTTL\": {\n          \"type\": \"integer\",\n          \"description\": \"Registration TTL in seconds.\",\n          \"default\": 90\n        },\n        \"registerInterval\": {\n          \"type\": \"integer\",\n          \"description\": \"Registration refresh interval in seconds.\",\n          \"default\": 30\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"client\": {\n      \"type\": \"object\",\n      \"description\": \"Client configuration options.\",\n      \"properties\": {\n        \"contentType\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Default content type for requests.\",\n          \"default\": \"application/protobuf\"\n        },\n        \"retries\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of retries on failure.\",\n          \"default\": 1\n        },\n        \"requestTimeout\": {\n          \"type\": \"string\",\n          \"description\": \"Request timeout duration (e.g., 5s).\",\n          \"default\": \"5s\"\n        },\n        \"poolSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Connection pool size.\",\n          \"default\": 1\n        },\n        \"poolTTL\": {\n          \"type\": \"string\",\n          \"description\": \"Connection pool TTL.\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"registry\": {\n      \"type\": \"object\",\n      \"description\": \"Service registry configuration.\",\n      \"properties\": {\n        \"type\": {\n          \"\
  type\": \"string\",\n          \"description\": \"Registry implementation.\",\n          \"enum\": [\"mdns\", \"consul\", \"etcd\", \"kubernetes\", \"memory\"],\n          \"default\": \"mdns\"\n        },\n        \"addresses\": {\n          \"type\": \"array\",\n          \"description\": \"Registry server addresses.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"broker\": {\n      \"type\": \"object\",\n      \"description\": \"Message broker configuration.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Broker implementation.\",\n          \"enum\": [\"http\", \"nats\", \"rabbitmq\", \"redis\", \"kafka\", \"memory\"],\n          \"default\": \"http\"\n        },\n        \"addresses\": {\n          \"type\": \"array\",\n          \"description\": \"Broker server addresses.\",\n          \"items\": {\n            \"type\"\
  : \"string\"\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"transport\": {\n      \"type\": \"object\",\n      \"description\": \"Transport layer configuration.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Transport implementation.\",\n          \"enum\": [\"http\", \"grpc\", \"tcp\", \"quic\", \"memory\"],\n          \"default\": \"http\"\n        },\n        \"addresses\": {\n          \"type\": \"array\",\n          \"description\": \"Transport addresses.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"selector\": {\n      \"type\": \"object\",\n      \"description\": \"Service selector / load balancer configuration.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Selector strategy.\",\n          \"enum\": [\"roundrobin\"\
  , \"random\", \"cache\"],\n          \"default\": \"cache\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"runtime\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime configuration.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Runtime implementation.\",\n          \"enum\": [\"local\", \"kubernetes\"],\n          \"default\": \"local\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"Source for the runtime.\"\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/go-micro/refs/heads/main/json-schema/go-micro-options.json
tags:
- Distributed Systems
- Frameworks
- Go
- Golang
- Microservices
- RPC
- Service Discovery
title: Go Micro Service Options
---
