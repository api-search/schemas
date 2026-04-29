---
description: The partition key definition.
layout: schema
name: PartitionKeyDefinition
properties_list:
- description: List of paths using which data within the container can be partitioned.
  name: paths
  type: array
- description: The algorithm used for partitioning.
  name: kind
  type: string
- description: The version of the partition key definition.
  name: version
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-partition-key-definition-schema.json
slug: azure-cosmos-db-partition-key-definition
source_filename: azure-cosmos-db-partition-key-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PartitionKeyDefinition\",\n  \"type\": \"object\",\n  \"description\": \"The partition key definition.\",\n  \"properties\": {\n    \"paths\": {\n      \"type\": \"array\",\n      \"description\": \"List of paths using which data within the container can be partitioned.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The algorithm used for partitioning.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the partition key definition.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-partition-key-definition-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: PartitionKeyDefinition
---
