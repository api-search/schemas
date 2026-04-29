---
description: The container Http Get settings, for liveness or readiness probe
layout: schema
name: ContainerHttpGet
properties_list:
- description: The path to probe.
  name: path
  type: string
- description: The port number to probe.
  name: port
  type: integer
- description: The scheme.
  name: scheme
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-http-get-schema.json
slug: azure-container-instances-container-http-get
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-http-get-schema.json\",\n  \"title\": \"ContainerHttpGet\",\n  \"description\": \"The container Http Get settings, for liveness or readiness probe\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"description\": \"The path to probe.\",\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"description\": \"The port number to probe.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"scheme\": {\n      \"description\": \"The scheme.\",\n      \"enum\": [\n        \"http\",\n        \"https\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"port\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-http-get-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerHttpGet
---
