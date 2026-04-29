---
description: Specifies the configuration for cold storage options such as enabled
layout: schema
name: ColdStorageOptions
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-cold-storage-options-schema.json
slug: openapi-cold-storage-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-cold-storage-options-schema.json\",\n  \"title\": \"ColdStorageOptions\",\n  \"description\": \"Specifies the configuration for cold storage options such as enabled\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Enable cold storage option. Accepted values true or false\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-cold-storage-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ColdStorageOptions
---
