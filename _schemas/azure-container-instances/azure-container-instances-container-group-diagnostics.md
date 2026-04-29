---
description: Container group diagnostic information.
layout: schema
name: ContainerGroupDiagnostics
properties_list:
- description: Container group log analytics information.
  name: logAnalytics
  type: object
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-group-diagnostics-schema.json
slug: azure-container-instances-container-group-diagnostics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-group-diagnostics-schema.json\",\n  \"title\": \"ContainerGroupDiagnostics\",\n  \"description\": \"Container group diagnostic information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logAnalytics\": {\n      \"$ref\": \"#/definitions/LogAnalytics\",\n      \"description\": \"Container group log analytics information.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-group-diagnostics-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerGroupDiagnostics
---
