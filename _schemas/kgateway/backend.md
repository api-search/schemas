---
description: Backend defines a routable backend such as an AI provider, AWS Lambda function, or static server for use by Gateways.
layout: schema
name: kgateway Backend
properties_list:
- description: API version for the Backend resource.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: Standard Kubernetes object metadata.
  name: metadata
  type: object
- description: BackendSpec defines the desired state of a Backend.
  name: spec
  type: object
provider_name: Kgateway
provider_slug: kgateway
schema_file: json-schema/backend.json
slug: backend
source_filename: backend.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kgateway/blob/main/json-schema/backend.json\",\n  \"title\": \"kgateway Backend\",\n  \"description\": \"Backend defines a routable backend such as an AI provider, AWS Lambda function, or static server for use by Gateways.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"gateway.kgateway.dev/v1alpha1\",\n      \"description\": \"API version for the Backend resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"Backend\",\n      \"description\": \"Resource kind.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the Backend resource.\"\n        },\n        \"namespace\":\
  \ {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the Backend resource.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"BackendSpec defines the desired state of a Backend.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the backend.\",\n          \"enum\": [\"Static\", \"AWS\", \"AI\"]\n        },\n        \"static\": {\n          \"type\": \"object\",\n          \"description\": \"Static backend configuration.\",\n          \"properties\": {\n            \"hosts\": {\n              \"type\": \"array\",\n              \"description\": \"List\
  \ of static hosts.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"host\": {\n                    \"type\": \"string\",\n                    \"description\": \"Hostname or IP address.\"\n                  },\n                  \"port\": {\n                    \"type\": \"integer\",\n                    \"description\": \"Port number.\"\n                  },\n                  \"tls\": {\n                    \"type\": \"object\",\n                    \"description\": \"TLS configuration for the host.\",\n                    \"properties\": {\n                      \"sni\": { \"type\": \"string\" }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"aws\": {\n          \"type\": \"object\",\n          \"description\": \"AWS Lambda backend configuration.\",\n          \"properties\": {\n            \"region\": {\n              \"type\"\
  : \"string\",\n              \"description\": \"AWS region.\"\n            },\n            \"lambdaFunctionName\": {\n              \"type\": \"string\",\n              \"description\": \"Name of the AWS Lambda function.\"\n            },\n            \"accountId\": {\n              \"type\": \"string\",\n              \"description\": \"AWS account ID.\"\n            },\n            \"roleArn\": {\n              \"type\": \"string\",\n              \"description\": \"ARN of the IAM role to assume.\"\n            }\n          }\n        },\n        \"ai\": {\n          \"type\": \"object\",\n          \"description\": \"AI provider backend configuration.\",\n          \"properties\": {\n            \"provider\": {\n              \"type\": \"object\",\n              \"description\": \"Configuration for the LLM provider.\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"openai\", \"azure\", \"gemini\"\
  , \"mistral\"]\n                },\n                \"openai\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"authToken\": { \"$ref\": \"#/$defs/AuthToken\" }\n                  }\n                },\n                \"azure\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"endpoint\": { \"type\": \"string\" },\n                    \"deploymentName\": { \"type\": \"string\" },\n                    \"apiVersion\": { \"type\": \"string\" },\n                    \"authToken\": { \"$ref\": \"#/$defs/AuthToken\" }\n                  }\n                },\n                \"gemini\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"authToken\": { \"$ref\": \"#/$defs/AuthToken\" }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"AuthToken\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"secretRef\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"namespace\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/json-schema/backend.json
tags:
- Gateways
title: kgateway Backend
---
