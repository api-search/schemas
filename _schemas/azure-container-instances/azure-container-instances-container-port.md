---
description: The port exposed on the container instance.
layout: schema
name: ContainerPort
properties_list:
- description: The port number exposed within the container group.
  name: port
  type: integer
- description: The protocol associated with the port.
  name: protocol
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-port-schema.json
slug: azure-container-instances-container-port
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-port-schema.json\",\n  \"title\": \"ContainerPort\",\n  \"description\": \"The port exposed on the container instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"description\": \"The port number exposed within the container group.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"protocol\": {\n      \"description\": \"The protocol associated with the port.\",\n      \"enum\": [\n        \"TCP\",\n        \"UDP\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ContainerNetworkProtocol\"\n      }\n    }\n  },\n  \"required\": [\n    \"port\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-port-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerPort
---
