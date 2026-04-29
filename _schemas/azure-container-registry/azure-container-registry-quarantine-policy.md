---
description: The quarantine policy for a container registry.
layout: schema
name: QuarantinePolicy
properties_list:
- description: The value that indicates whether the policy is enabled or not.
  name: status
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-quarantine-policy-schema.json
slug: azure-container-registry-quarantine-policy
source_filename: azure-container-registry-quarantine-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-quarantine-policy-schema.json\",\n  \"title\": \"QuarantinePolicy\",\n  \"description\": \"The quarantine policy for a container registry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"default\": \"disabled\",\n      \"description\": \"The value that indicates whether the policy is enabled or not.\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"PolicyStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-quarantine-policy-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: QuarantinePolicy
---
