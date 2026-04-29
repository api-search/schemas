---
description: The retention policy.
layout: schema
name: RetentionPolicy
properties_list:
- description: Indicates whether a retention policy is enabled.
  name: Enabled
  type: boolean
- description: The number of days that metrics or logging data should be retained.
  name: Days
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-retention-policy-schema.json
slug: azure-blob-storage-retention-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RetentionPolicy\",\n  \"type\": \"object\",\n  \"description\": \"The retention policy.\",\n  \"properties\": {\n    \"Enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a retention policy is enabled.\"\n    },\n    \"Days\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days that metrics or logging data should be retained.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-retention-policy-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: RetentionPolicy
---
