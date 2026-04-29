---
description: StorageTypes represents the list of storage related types and their attributes that are available for given InstanceType.
layout: schema
name: StorageType
properties_list:
- description: ''
  name: StorageTypeName
  type: object
- description: ''
  name: StorageSubTypeName
  type: object
- description: ''
  name: StorageTypeLimits
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-storage-type-schema.json
slug: openapi-storage-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-storage-type-schema.json\",\n  \"title\": \"StorageType\",\n  \"description\": \"StorageTypes represents the list of storage related types and their attributes that are available for given InstanceType. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StorageTypeName\": {\n      \"$ref\": \"#/components/schemas/StorageTypeName\"\n    },\n    \"StorageSubTypeName\": {\n      \"$ref\": \"#/components/schemas/StorageSubTypeName\"\n    },\n    \"StorageTypeLimits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageTypeLimitList\"\n        },\n        {\n          \"description\": \"List of limits that are applicable for given storage type. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-storage-type-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: StorageType
---
