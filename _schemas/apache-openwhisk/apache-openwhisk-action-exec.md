---
description: ActionExec schema from Apache OpenWhisk
layout: schema
name: ActionExec
properties_list:
- description: Runtime kind
  name: kind
  type: string
- description: Inline function source code
  name: code
  type: string
- description: Docker image for blackbox/docker kind
  name: image
  type: string
- description: Sequence of action names (for sequence kind)
  name: components
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-action-exec-schema.json
slug: apache-openwhisk-action-exec
source_filename: apache-openwhisk-action-exec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-exec-schema.json\",\n  \"title\": \"ActionExec\",\n  \"description\": \"ActionExec schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Runtime kind\",\n      \"example\": \"nodejs:18\",\n      \"enum\": [\n        \"nodejs:18\",\n        \"nodejs:20\",\n        \"python:3\",\n        \"java:8\",\n        \"go:1.20\",\n        \"php:8.0\",\n        \"ruby:2.5\",\n        \"swift:5.7\",\n        \"dotnet:2.2\",\n        \"docker\",\n        \"blackbox\",\n        \"sequence\"\n      ]\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Inline function source code\",\n      \"example\": \"function main(params) { return { message: 'Hello ' + (params.name ||\
  \ 'World') }; }\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Docker image for blackbox/docker kind\",\n      \"example\": \"openwhisk/nodejs18action\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Sequence of action names (for sequence kind)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-action-exec-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActionExec
---
