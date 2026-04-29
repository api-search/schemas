---
description: Specifies the node-to-node encryption options.
layout: schema
name: NodeToNodeEncryptionOptions
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-node-to-node-encryption-options-schema.json
slug: openapi-node-to-node-encryption-options
source_filename: openapi-node-to-node-encryption-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-node-to-node-encryption-options-schema.json\",\n  \"title\": \"NodeToNodeEncryptionOptions\",\n  \"description\": \"Specifies the node-to-node encryption options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specify true to enable node-to-node encryption.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-node-to-node-encryption-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: NodeToNodeEncryptionOptions
---
