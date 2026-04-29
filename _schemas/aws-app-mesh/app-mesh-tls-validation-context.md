---
description: An object that represents how the proxy will validate its peer during Transport Layer Security (TLS) negotiation.
layout: schema
name: TlsValidationContext
properties_list:
- description: ''
  name: subjectAlternativeNames
  type: object
- description: ''
  name: trust
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tls-validation-context-schema.json
slug: app-mesh-tls-validation-context
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"subjectAlternativeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectAlternativeNames\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the SANs for a Transport Layer Security (TLS) validation context. If you don't specify SANs on the <i>terminating</i> mesh endpoint, the Envoy proxy for that node doesn't verify the SAN on a peer client certificate. If you don't specify SANs on the <i>originating</i> mesh endpoint, the SAN on the certificate provided by the terminating endpoint must match the mesh endpoint service discovery configuration. Since SPIRE vended certificates have a SPIFFE ID as a name, you must set the SAN since the name doesn't match the service discovery name.\"\n        }\n      ]\n    },\n    \"trust\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TlsValidationContextTrust\"\n        },\n\
  \        {\n          \"description\": \"A reference to where to retrieve the trust chain when validating a peer\\u2019s Transport Layer Security (TLS) certificate.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"trust\"\n  ],\n  \"description\": \"An object that represents how the proxy will validate its peer during Transport Layer Security (TLS) negotiation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tls-validation-context-schema.json\",\n  \"title\": \"TlsValidationContext\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tls-validation-context-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TlsValidationContext
---
