---
description: The environment variable to set within the container instance.
layout: schema
name: EnvironmentVariable
properties_list:
- description: The name of the environment variable.
  name: name
  type: string
- description: The value of the secure environment variable.
  name: secureValue
  type: string
- description: The value of the environment variable.
  name: value
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-environment-variable-schema.json
slug: azure-container-instances-environment-variable
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-environment-variable-schema.json\",\n  \"title\": \"EnvironmentVariable\",\n  \"description\": \"The environment variable to set within the container instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the environment variable.\",\n      \"type\": \"string\"\n    },\n    \"secureValue\": {\n      \"description\": \"The value of the secure environment variable.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The value of the environment variable.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-environment-variable-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: EnvironmentVariable
---
