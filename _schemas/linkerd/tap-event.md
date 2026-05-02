---
description: A real-time traffic event captured by the Linkerd Tap API, containing source and destination metadata, proxy direction, and HTTP request/response details.
layout: schema
name: Linkerd Tap Event
properties_list:
- description: Source TCP address of the request.
  name: source
  type: object
- description: Metadata labels for the source workload.
  name: source_meta
  type: object
- description: Destination TCP address of the request.
  name: destination
  type: object
- description: Metadata labels for the destination workload.
  name: destination_meta
  type: object
- description: Metadata labels for the matched route.
  name: route_meta
  type: object
- description: Direction of the proxied request.
  name: proxy_direction
  type: string
- description: Initial request metadata when a new request begins.
  name: request_init
  type: object
- description: Initial response metadata when headers are received.
  name: response_init
  type: object
- description: Final response metadata when the stream completes.
  name: response_end
  type: object
provider_name: Linkerd
provider_slug: linkerd
schema_file: json-schema/tap-event.json
slug: tap-event
source_filename: tap-event.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/linkerd/blob/main/json-schema/tap-event.json\",\n  \"title\": \"Linkerd Tap Event\",\n  \"description\": \"A real-time traffic event captured by the Linkerd Tap API, containing source and destination metadata, proxy direction, and HTTP request/response details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"$ref\": \"#/$defs/TcpAddress\",\n      \"description\": \"Source TCP address of the request.\"\n    },\n    \"source_meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata labels for the source workload.\",\n      \"properties\": {\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"destination\": {\n      \"$ref\": \"#/$defs/TcpAddress\",\n      \"description\": \"Destination TCP address\
  \ of the request.\"\n    },\n    \"destination_meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata labels for the destination workload.\",\n      \"properties\": {\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"route_meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata labels for the matched route.\",\n      \"properties\": {\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"proxy_direction\": {\n      \"type\": \"string\",\n      \"description\": \"Direction of the proxied request.\",\n      \"enum\": [\"INBOUND\", \"OUTBOUND\"]\n    },\n    \"request_init\": {\n      \"type\": \"object\",\n      \"description\": \"Initial request metadata when a new request begins.\",\n      \"properties\"\
  : {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique stream identifier for this request.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method of the request.\"\n        },\n        \"scheme\": {\n          \"type\": \"string\",\n          \"description\": \"URI scheme (http or https).\"\n        },\n        \"authority\": {\n          \"type\": \"string\",\n          \"description\": \"Authority (Host header) of the request.\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Request path.\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"HTTP request headers.\"\n        }\n      }\n    },\n    \"response_init\": {\n      \"type\": \"object\",\n      \"description\": \"Initial response metadata when headers\
  \ are received.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique stream identifier matching the request.\"\n        },\n        \"http_status\": {\n          \"type\": \"integer\",\n          \"description\": \"HTTP response status code.\"\n        },\n        \"latency_ns\": {\n          \"type\": \"integer\",\n          \"description\": \"Time to first response byte in nanoseconds.\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"HTTP response headers.\"\n        }\n      }\n    },\n    \"response_end\": {\n      \"type\": \"object\",\n      \"description\": \"Final response metadata when the stream completes.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique stream identifier matching the request.\"\n        },\n\
  \        \"grpc_status\": {\n          \"type\": \"integer\",\n          \"description\": \"gRPC status code if applicable.\"\n        },\n        \"duration_ns\": {\n          \"type\": \"integer\",\n          \"description\": \"Total stream duration in nanoseconds.\"\n        },\n        \"response_bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Total response body bytes.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"TcpAddress\": {\n      \"type\": \"object\",\n      \"description\": \"A TCP address consisting of an IP and port.\",\n      \"properties\": {\n        \"ip\": {\n          \"type\": \"string\",\n          \"description\": \"IP address.\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"Port number.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/json-schema/tap-event.json
tags:
- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh
title: Linkerd Tap Event
---
