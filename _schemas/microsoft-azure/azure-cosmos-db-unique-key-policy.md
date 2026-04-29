---
description: The unique key policy configuration.
layout: schema
name: UniqueKeyPolicy
properties_list:
- description: List of unique keys for the container.
  name: uniqueKeys
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-unique-key-policy-schema.json
slug: azure-cosmos-db-unique-key-policy
source_filename: azure-cosmos-db-unique-key-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UniqueKeyPolicy\",\n  \"type\": \"object\",\n  \"description\": \"The unique key policy configuration.\",\n  \"properties\": {\n    \"uniqueKeys\": {\n      \"type\": \"array\",\n      \"description\": \"List of unique keys for the container.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-unique-key-policy-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: UniqueKeyPolicy
---
