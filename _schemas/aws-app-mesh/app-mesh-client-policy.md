---
description: An object that represents a client policy.
layout: schema
name: ClientPolicy
properties_list:
- description: ''
  name: tls
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-client-policy-schema.json
slug: app-mesh-client-policy
source_filename: app-mesh-client-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"tls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientPolicyTls\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a Transport Layer Security (TLS) client policy.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents a client policy.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-client-policy-schema.json\",\n  \"title\": \"ClientPolicy\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-client-policy-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ClientPolicy
---
