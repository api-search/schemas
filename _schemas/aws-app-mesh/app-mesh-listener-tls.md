---
description: An object that represents the Transport Layer Security (TLS) properties for a listener.
layout: schema
name: ListenerTls
properties_list:
- description: ''
  name: certificate
  type: object
- description: ''
  name: mode
  type: object
- description: ''
  name: validation
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-listener-tls-schema.json
slug: app-mesh-listener-tls
source_filename: app-mesh-listener-tls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerTlsCertificate\"\n        },\n        {\n          \"description\": \"A reference to an object that represents a listener's Transport Layer Security (TLS) certificate.\"\n        }\n      ]\n    },\n    \"mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerTlsMode\"\n        },\n        {\n          \"description\": \"<p>Specify one of the following modes.</p> <ul> <li> <p> <b/>STRICT \\u2013 Listener only accepts connections with TLS enabled. </p> </li> <li> <p> <b/>PERMISSIVE \\u2013 Listener accepts connections with or without TLS enabled.</p> </li> <li> <p> <b/>DISABLED \\u2013 Listener only accepts connections without TLS. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"validation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerTlsValidationContext\"\
  \n        },\n        {\n          \"description\": \"A reference to an object that represents a listener's Transport Layer Security (TLS) validation context.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"certificate\",\n    \"mode\"\n  ],\n  \"description\": \"An object that represents the Transport Layer Security (TLS) properties for a listener.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-tls-schema.json\",\n  \"title\": \"ListenerTls\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-listener-tls-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: ListenerTls
---
