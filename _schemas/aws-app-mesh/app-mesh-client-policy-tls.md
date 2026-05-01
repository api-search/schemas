---
description: A reference to an object that represents a Transport Layer Security (TLS) client policy.
layout: schema
name: ClientPolicyTls
properties_list:
- description: ''
  name: certificate
  type: object
- description: ''
  name: enforce
  type: object
- description: ''
  name: ports
  type: object
- description: ''
  name: validation
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-client-policy-tls-schema.json
slug: app-mesh-client-policy-tls
source_filename: app-mesh-client-policy-tls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientTlsCertificate\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a client's TLS certificate.\"\n        }\n      ]\n    },\n    \"enforce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the policy is enforced. The default is <code>True</code>, if a value isn't specified.\"\n        }\n      ]\n    },\n    \"ports\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortSet\"\n        },\n        {\n          \"description\": \"One or more ports that the policy is enforced for.\"\n        }\n      ]\n    },\n    \"validation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TlsValidationContext\"\n        },\n        {\n \
  \         \"description\": \"A reference to an object that represents a TLS validation context.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"validation\"\n  ],\n  \"description\": \"A reference to an object that represents a Transport Layer Security (TLS) client policy.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-client-policy-tls-schema.json\",\n  \"title\": \"ClientPolicyTls\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-client-policy-tls-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ClientPolicyTls
---
