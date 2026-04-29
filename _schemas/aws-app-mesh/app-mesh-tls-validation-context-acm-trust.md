---
description: An object that represents a Transport Layer Security (TLS) validation context trust for an Certificate Manager certificate.
layout: schema
name: TlsValidationContextAcmTrust
properties_list:
- description: ''
  name: certificateAuthorityArns
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tls-validation-context-acm-trust-schema.json
slug: app-mesh-tls-validation-context-acm-trust
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateAuthorityArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityArns\"\n        },\n        {\n          \"description\": \"One or more ACM Amazon Resource Name (ARN)s.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"certificateAuthorityArns\"\n  ],\n  \"description\": \"An object that represents a Transport Layer Security (TLS) validation context trust for an Certificate Manager certificate.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tls-validation-context-acm-trust-schema.json\",\n  \"title\": \"TlsValidationContextAcmTrust\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tls-validation-context-acm-trust-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TlsValidationContextAcmTrust
---
