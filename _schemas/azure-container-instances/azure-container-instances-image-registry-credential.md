---
description: Image registry credential.
layout: schema
name: ImageRegistryCredential
properties_list:
- description: The password for the private registry.
  name: password
  type: string
- description: The Docker image registry server without a protocol such as "http" and "https".
  name: server
  type: string
- description: The username for the private registry.
  name: username
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-image-registry-credential-schema.json
slug: azure-container-instances-image-registry-credential
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-image-registry-credential-schema.json\",\n  \"title\": \"ImageRegistryCredential\",\n  \"description\": \"Image registry credential.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"password\": {\n      \"description\": \"The password for the private registry.\",\n      \"type\": \"string\"\n    },\n    \"server\": {\n      \"description\": \"The Docker image registry server without a protocol such as \\\"http\\\" and \\\"https\\\".\",\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"description\": \"The username for the private registry.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"server\",\n    \"username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-image-registry-credential-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ImageRegistryCredential
---
