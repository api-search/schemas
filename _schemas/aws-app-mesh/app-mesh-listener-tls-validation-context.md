---
description: An object that represents a listener's Transport Layer Security (TLS) validation context.
layout: schema
name: ListenerTlsValidationContext
properties_list:
- description: ''
  name: subjectAlternativeNames
  type: object
- description: ''
  name: trust
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-listener-tls-validation-context-schema.json
slug: app-mesh-listener-tls-validation-context
source_filename: app-mesh-listener-tls-validation-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"subjectAlternativeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectAlternativeNames\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the SANs for a listener's Transport Layer Security (TLS) validation context.\"\n        }\n      ]\n    },\n    \"trust\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerTlsValidationContextTrust\"\n        },\n        {\n          \"description\": \"A reference to where to retrieve the trust chain when validating a peer\\u2019s Transport Layer Security (TLS) certificate.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"trust\"\n  ],\n  \"description\": \"An object that represents a listener's Transport Layer Security (TLS) validation context.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-tls-validation-context-schema.json\"\
  ,\n  \"title\": \"ListenerTlsValidationContext\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-tls-validation-context-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ListenerTlsValidationContext
---
