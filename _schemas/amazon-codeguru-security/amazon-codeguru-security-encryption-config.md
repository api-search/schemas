---
description: Information about account-level configuration.
layout: schema
name: EncryptionConfig
properties_list:
- description: ''
  name: kmsKeyArn
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-encryption-config-schema.json
slug: amazon-codeguru-security-encryption-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-encryption-config-schema.json\",\n  \"title\": \"EncryptionConfig\",\n  \"description\": \"Information about account-level configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The KMS key ARN to use for encryption. This must be provided as a header when uploading your code resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-encryption-config-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: EncryptionConfig
---
