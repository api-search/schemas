---
description: PutEncryptionConfigResult schema from Amazon X-Ray API
layout: schema
name: PutEncryptionConfigResult
properties_list:
- description: ''
  name: EncryptionConfig
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-put-encryption-config-result-schema.json
slug: xray-put-encryption-config-result
source_filename: xray-put-encryption-config-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncryptionConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfig\"\n        },\n        {\n          \"description\": \"The new encryption configuration.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutEncryptionConfigResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-encryption-config-result-schema.json\",\n  \"description\": \"PutEncryptionConfigResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-encryption-config-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: PutEncryptionConfigResult
---
