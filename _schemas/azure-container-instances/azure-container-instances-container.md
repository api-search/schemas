---
description: A container instance.
layout: schema
name: Container
properties_list:
- description: The user-provided name of the container instance.
  name: name
  type: string
- description: The properties of the container instance.
  name: properties
  type: object
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-schema.json
slug: azure-container-instances-container
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-schema.json\",\n  \"title\": \"Container\",\n  \"description\": \"A container instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The user-provided name of the container instance.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/ContainerProperties\",\n      \"description\": \"The properties of the container instance.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"required\": [\n    \"properties\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: Container
---
