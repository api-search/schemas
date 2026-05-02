---
description: HTTPListenerPolicy applies policies to all HTTP and HTTPS listeners on a Gateway, configuring the Envoy HttpConnectionManager and other listener-level settings.
layout: schema
name: kgateway HTTPListenerPolicy
properties_list:
- description: API version for the HTTPListenerPolicy resource.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: Standard Kubernetes object metadata.
  name: metadata
  type: object
- description: HTTPListenerPolicySpec defines the desired state of an HTTPListenerPolicy.
  name: spec
  type: object
provider_name: Kgateway
provider_slug: kgateway
schema_file: json-schema/http-listener-policy.json
slug: http-listener-policy
source_filename: http-listener-policy.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kgateway/blob/main/json-schema/http-listener-policy.json\",\n  \"title\": \"kgateway HTTPListenerPolicy\",\n  \"description\": \"HTTPListenerPolicy applies policies to all HTTP and HTTPS listeners on a Gateway, configuring the Envoy HttpConnectionManager and other listener-level settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"gateway.kgateway.dev/v1alpha1\",\n      \"description\": \"API version for the HTTPListenerPolicy resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"HTTPListenerPolicy\",\n      \"description\": \"Resource kind.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n       \
  \   \"description\": \"Name of the HTTPListenerPolicy resource.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the HTTPListenerPolicy resource.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"HTTPListenerPolicySpec defines the desired state of an HTTPListenerPolicy.\",\n      \"properties\": {\n        \"targetRefs\": {\n          \"type\": \"array\",\n          \"description\": \"References to the Gateway listeners to which this policy applies.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"group\": { \"type\"\
  : \"string\" },\n              \"kind\": { \"type\": \"string\" },\n              \"name\": { \"type\": \"string\" }\n            },\n            \"required\": [\"kind\", \"name\"]\n          }\n        },\n        \"accessLogging\": {\n          \"type\": \"object\",\n          \"description\": \"Access logging configuration.\"\n        },\n        \"buffer\": {\n          \"type\": \"object\",\n          \"description\": \"Request buffering configuration.\",\n          \"properties\": {\n            \"maxRequestBytes\": {\n              \"type\": \"integer\",\n              \"description\": \"Maximum request body size in bytes.\"\n            }\n          }\n        },\n        \"celValidation\": {\n          \"type\": \"object\",\n          \"description\": \"CEL-based request validation.\",\n          \"properties\": {\n            \"rules\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n\
  \                  \"expression\": {\n                    \"type\": \"string\",\n                    \"description\": \"CEL expression to evaluate.\"\n                  },\n                  \"action\": {\n                    \"type\": \"string\",\n                    \"enum\": [\"Deny\", \"Allow\"]\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"basicAuth\": {\n          \"type\": \"object\",\n          \"description\": \"Basic authentication configuration.\",\n          \"properties\": {\n            \"credentialsSecretRef\": {\n              \"type\": \"object\",\n              \"description\": \"Reference to a Kubernetes secret containing htpasswd-format credentials.\",\n              \"properties\": {\n                \"name\": { \"type\": \"string\" },\n                \"namespace\": { \"type\": \"string\" }\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\"targetRefs\"]\n    }\n \
  \ }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/json-schema/http-listener-policy.json
tags:
- Gateways
title: kgateway HTTPListenerPolicy
---
