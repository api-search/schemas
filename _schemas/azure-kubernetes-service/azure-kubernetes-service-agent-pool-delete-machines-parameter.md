---
description: The parameters for deleting machines in an agent pool.
layout: schema
name: AgentPoolDeleteMachinesParameter
properties_list:
- description: The list of machine names to delete.
  name: machineNames
  type: array
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-agent-pool-delete-machines-parameter-schema.json
slug: azure-kubernetes-service-agent-pool-delete-machines-parameter
source_filename: azure-kubernetes-service-agent-pool-delete-machines-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPoolDeleteMachinesParameter\",\n  \"type\": \"object\",\n  \"description\": \"The parameters for deleting machines in an agent pool.\",\n  \"properties\": {\n    \"machineNames\": {\n      \"type\": \"array\",\n      \"description\": \"The list of machine names to delete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-delete-machines-parameter-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: AgentPoolDeleteMachinesParameter
---
