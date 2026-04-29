---
description: UpdateAccountConfigurationRequest schema from Amazon CodeGuru Security
layout: schema
name: UpdateAccountConfigurationRequest
properties_list:
- description: ''
  name: encryptionConfig
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-update-account-configuration-request-schema.json
slug: amazon-codeguru-security-update-account-configuration-request
source_filename: amazon-codeguru-security-update-account-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-update-account-configuration-request-schema.json\",\n  \"title\": \"UpdateAccountConfigurationRequest\",\n  \"description\": \"UpdateAccountConfigurationRequest schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfig\"\n        },\n        {\n          \"description\": \"The KMS key ARN you want to use for encryption. Defaults to service-side encryption if missing.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"encryptionConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-update-account-configuration-request-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: UpdateAccountConfigurationRequest
---
