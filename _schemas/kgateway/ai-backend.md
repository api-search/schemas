---
description: AIBackend configures AI provider backends with support for LLM providers such as OpenAI, Azure OpenAI, Gemini, and Mistral, including priority-based routing groups.
layout: schema
name: kgateway AIBackend
properties_list:
- description: API version for the AIBackend resource.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: Standard Kubernetes object metadata.
  name: metadata
  type: object
- description: AIBackendSpec defines the desired state of an AIBackend.
  name: spec
  type: object
provider_name: Kgateway
provider_slug: kgateway
schema_file: json-schema/ai-backend.json
slug: ai-backend
source_filename: ai-backend.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kgateway/blob/main/json-schema/ai-backend.json\",\n  \"title\": \"kgateway AIBackend\",\n  \"description\": \"AIBackend configures AI provider backends with support for LLM providers such as OpenAI, Azure OpenAI, Gemini, and Mistral, including priority-based routing groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"gateway.kgateway.dev/v1alpha1\",\n      \"description\": \"API version for the AIBackend resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"AIBackend\",\n      \"description\": \"Resource kind.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the\
  \ AIBackend resource.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the AIBackend resource.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"AIBackendSpec defines the desired state of an AIBackend.\",\n      \"properties\": {\n        \"provider\": {\n          \"type\": \"object\",\n          \"description\": \"Configuration for the LLM provider.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The type of LLM provider.\",\n              \"enum\": [\"openai\", \"azure\", \"gemini\", \"mistral\"\
  ]\n            },\n            \"openai\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"model\": {\n                  \"type\": \"string\",\n                  \"description\": \"Model name to use.\"\n                },\n                \"authToken\": { \"$ref\": \"#/$defs/AuthToken\" }\n              }\n            },\n            \"azure\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"endpoint\": { \"type\": \"string\" },\n                \"deploymentName\": { \"type\": \"string\" },\n                \"apiVersion\": { \"type\": \"string\" },\n                \"authToken\": { \"$ref\": \"#/$defs/AuthToken\" }\n              }\n            },\n            \"gemini\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"model\": { \"type\": \"string\" },\n                \"authToken\": { \"$ref\": \"#/$defs/AuthToken\" }\n              }\n            }\n     \
  \     }\n        },\n        \"groups\": {\n          \"type\": \"array\",\n          \"description\": \"List of groups in priority order where each group defines a set of LLM providers.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"priority\": {\n                \"type\": \"integer\",\n                \"description\": \"Priority of this group (lower is higher priority).\"\n              },\n              \"backends\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"backendRef\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"name\": { \"type\": \"string\" },\n                        \"namespace\": { \"type\": \"string\" }\n                      }\n                    },\n                    \"weight\": {\n                      \"type\"\
  : \"integer\",\n                      \"description\": \"Weight for load balancing within the group.\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"AuthToken\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"secretRef\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"namespace\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/json-schema/ai-backend.json
tags:
- Gateways
title: kgateway AIBackend
---
