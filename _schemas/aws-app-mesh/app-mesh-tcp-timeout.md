---
description: An object that represents types of timeouts.
layout: schema
name: TcpTimeout
properties_list:
- description: ''
  name: idle
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-tcp-timeout-schema.json
slug: app-mesh-tcp-timeout
source_filename: app-mesh-tcp-timeout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"idle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"An object that represents an idle timeout. An idle timeout bounds the amount of time that a connection may be idle. The default value is none.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents types of timeouts. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tcp-timeout-schema.json\",\n  \"title\": \"TcpTimeout\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-tcp-timeout-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: TcpTimeout
---
