---
description: A configuration document that specifies encryption configuration settings.
layout: schema
name: EncryptionConfig
properties_list:
- description: ''
  name: KeyId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-encryption-config-schema.json
slug: xray-encryption-config
source_filename: xray-encryption-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the KMS key used for encryption, if applicable.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionStatus\"\n        },\n        {\n          \"description\": \"The encryption status. While the status is <code>UPDATING</code>, X-Ray may encrypt data with a combination of the new and old settings.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionType\"\n        },\n        {\n          \"description\": \"The type of encryption. Set to <code>KMS</code> for encryption with KMS keys. Set to <code>NONE</code> for default encryption.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A configuration document\
  \ that specifies encryption configuration settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EncryptionConfig\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-encryption-config-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-encryption-config-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: EncryptionConfig
---
