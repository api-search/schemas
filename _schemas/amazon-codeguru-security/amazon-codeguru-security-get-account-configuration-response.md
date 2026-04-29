---
description: GetAccountConfigurationResponse schema from Amazon CodeGuru Security
layout: schema
name: GetAccountConfigurationResponse
properties_list:
- description: ''
  name: encryptionConfig
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-get-account-configuration-response-schema.json
slug: amazon-codeguru-security-get-account-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-get-account-configuration-response-schema.json\",\n  \"title\": \"GetAccountConfigurationResponse\",\n  \"description\": \"GetAccountConfigurationResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptionConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfig\"\n        },\n        {\n          \"description\": \"An <code>EncryptionConfig</code> object that contains the KMS key ARN to use for encryption. By default, CodeGuru Security uses an AWS-managed key for encryption. To specify your own key, call <code>UpdateAccountConfiguration</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"encryptionConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-get-account-configuration-response-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: GetAccountConfigurationResponse
---
