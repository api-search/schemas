---
description: An object that represents an access log file.
layout: schema
name: VirtualGatewayFileAccessLog
properties_list:
- description: ''
  name: format
  type: object
- description: ''
  name: path
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-file-access-log-schema.json
slug: app-mesh-virtual-gateway-file-access-log
source_filename: app-mesh-virtual-gateway-file-access-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingFormat\"\n        },\n        {\n          \"description\": \"The specified format for the virtual gateway access logs. It can be either <code>json_format</code> or <code>text_format</code>.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilePath\"\n        },\n        {\n          \"description\": \"The file path to write access logs to. You can use <code>/dev/stdout</code> to send access logs to standard out and configure your Envoy container to use a log driver, such as <code>awslogs</code>, to export the access logs to a log storage service such as Amazon CloudWatch Logs. You can also specify a path in the Envoy container's file system to write the files to disk.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"path\"\n  ],\n  \"description\"\
  : \"An object that represents an access log file.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-file-access-log-schema.json\",\n  \"title\": \"VirtualGatewayFileAccessLog\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-file-access-log-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayFileAccessLog
---
