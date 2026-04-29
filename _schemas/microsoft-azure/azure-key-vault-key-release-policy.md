---
description: The policy rules under which the key can be exported.
layout: schema
name: KeyReleasePolicy
properties_list:
- description: Content type and version of key release policy.
  name: contentType
  type: string
- description: Defines whether the policy is immutable.
  name: immutable
  type: boolean
- description: Blob encoding the policy rules (base64url-encoded).
  name: data
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-key-release-policy-schema.json
slug: azure-key-vault-key-release-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyReleasePolicy\",\n  \"type\": \"object\",\n  \"description\": \"The policy rules under which the key can be exported.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Content type and version of key release policy.\"\n    },\n    \"immutable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Defines whether the policy is immutable.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Blob encoding the policy rules (base64url-encoded).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-key-release-policy-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: KeyReleasePolicy
---
