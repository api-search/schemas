---
description: Specifies the Encryption At Rest Options.
layout: schema
name: EncryptionAtRestOptions
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: KmsKeyId
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-encryption-at-rest-options-schema.json
slug: openapi-encryption-at-rest-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-encryption-at-rest-options-schema.json\",\n  \"title\": \"EncryptionAtRestOptions\",\n  \"description\": \"Specifies the Encryption At Rest Options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies the option to enable Encryption At Rest.\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \" Specifies the KMS Key ID for Encryption At Rest options.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-encryption-at-rest-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: EncryptionAtRestOptions
---
