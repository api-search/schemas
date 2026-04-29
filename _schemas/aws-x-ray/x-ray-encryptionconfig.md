---
description: ''
layout: schema
name: EncryptionConfig
properties_list:
- description: ''
  name: KeyId
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: Type
  type: string
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-encryptionconfig-schema.json
slug: x-ray-encryptionconfig
source_filename: x-ray-encryptionconfig-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EncryptionConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyId\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UPDATING\",\n        \"ACTIVE\"\n      ]\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"KMS\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/json-schema/x-ray-encryptionconfig-schema.json
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: EncryptionConfig
---
