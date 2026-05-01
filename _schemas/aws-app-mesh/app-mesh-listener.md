---
description: An object that represents a listener for a virtual node.
layout: schema
name: Listener
properties_list:
- description: ''
  name: connectionPool
  type: object
- description: ''
  name: healthCheck
  type: object
- description: ''
  name: outlierDetection
  type: object
- description: ''
  name: portMapping
  type: object
- description: ''
  name: timeout
  type: object
- description: ''
  name: tls
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-listener-schema.json
slug: app-mesh-listener
source_filename: app-mesh-listener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionPool\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualNodeConnectionPool\"\n        },\n        {\n          \"description\": \"The connection pool information for the listener.\"\n        }\n      ]\n    },\n    \"healthCheck\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckPolicy\"\n        },\n        {\n          \"description\": \"The health check information for the listener.\"\n        }\n      ]\n    },\n    \"outlierDetection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutlierDetection\"\n        },\n        {\n          \"description\": \"The outlier detection information for the listener.\"\n        }\n      ]\n    },\n    \"portMapping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortMapping\"\n        },\n        {\n          \"description\": \"The\
  \ port mapping information for the listener.\"\n        }\n      ]\n    },\n    \"timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerTimeout\"\n        },\n        {\n          \"description\": \"An object that represents timeouts for different protocols.\"\n        }\n      ]\n    },\n    \"tls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerTls\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the Transport Layer Security (TLS) properties for a listener.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"portMapping\"\n  ],\n  \"description\": \"An object that represents a listener for a virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-schema.json\",\n  \"title\": \"Listener\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: Listener
---
