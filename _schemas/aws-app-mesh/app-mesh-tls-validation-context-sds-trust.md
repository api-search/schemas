---
description: An object that represents a Transport Layer Security (TLS) Secret Discovery Service validation context trust. The proxy must be configured with a local SDS provider via a Unix Domain Socket. See App Mesh <a href="https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html">TLS documentation</a> for more info.
layout: schema
name: TlsValidationContextSdsTrust
properties_list:
- description: ''
  name: secretName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tls-validation-context-sds-trust-schema.json
slug: app-mesh-tls-validation-context-sds-trust
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"secretName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SdsSecretName\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the name of the secret for a Transport Layer Security (TLS) Secret Discovery Service validation context trust.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"secretName\"\n  ],\n  \"description\": \"An object that represents a Transport Layer Security (TLS) Secret Discovery Service validation context trust. The proxy must be configured with a local SDS provider via a Unix Domain Socket. See App Mesh <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html\\\">TLS documentation</a> for more info.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tls-validation-context-sds-trust-schema.json\"\
  ,\n  \"title\": \"TlsValidationContextSdsTrust\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tls-validation-context-sds-trust-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TlsValidationContextSdsTrust
---
