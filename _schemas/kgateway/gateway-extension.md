---
description: GatewayExtension integrates external services with a Gateway such as external auth, rate limiting, and external processing.
layout: schema
name: kgateway GatewayExtension
properties_list:
- description: API version for the GatewayExtension resource.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: Standard Kubernetes object metadata.
  name: metadata
  type: object
- description: GatewayExtensionSpec defines the desired state of a GatewayExtension.
  name: spec
  type: object
provider_name: Kgateway
provider_slug: kgateway
schema_file: json-schema/gateway-extension.json
slug: gateway-extension
source_filename: gateway-extension.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kgateway/blob/main/json-schema/gateway-extension.json\",\n  \"title\": \"kgateway GatewayExtension\",\n  \"description\": \"GatewayExtension integrates external services with a Gateway such as external auth, rate limiting, and external processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"gateway.kgateway.dev/v1alpha1\",\n      \"description\": \"API version for the GatewayExtension resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"GatewayExtension\",\n      \"description\": \"Resource kind.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the GatewayExtension\
  \ resource.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the GatewayExtension resource.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"GatewayExtensionSpec defines the desired state of a GatewayExtension.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the gateway extension.\",\n          \"enum\": [\"ExtAuth\", \"ExtProc\", \"RateLimit\"]\n        },\n        \"extAuth\": {\n          \"type\": \"object\",\n          \"description\": \"External auth extension configuration.\",\n          \"properties\"\
  : {\n            \"grpcService\": {\n              \"$ref\": \"#/$defs/GrpcService\"\n            }\n          }\n        },\n        \"extProc\": {\n          \"type\": \"object\",\n          \"description\": \"External processing extension configuration.\",\n          \"properties\": {\n            \"grpcService\": {\n              \"$ref\": \"#/$defs/GrpcService\"\n            }\n          }\n        },\n        \"rateLimit\": {\n          \"type\": \"object\",\n          \"description\": \"Rate limit extension configuration.\",\n          \"properties\": {\n            \"grpcService\": {\n              \"$ref\": \"#/$defs/GrpcService\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"GrpcService\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"backendRef\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"namespace\": { \"type\": \"string\" },\n   \
  \         \"port\": { \"type\": \"integer\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/json-schema/gateway-extension.json
tags:
- Gateways
title: kgateway GatewayExtension
---
