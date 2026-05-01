---
description: The customer-managed-key(CMK) used when creating a data store. If a customer owned key is not specified, an AWS owned key will be used for encryption.
layout: schema
name: KmsEncryptionConfig
properties_list:
- description: ''
  name: CmkType
  type: object
- description: ''
  name: KmsKeyId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-kms-encryption-config-schema.json
slug: healthlake-kms-encryption-config
source_filename: healthlake-kms-encryption-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-kms-encryption-config-schema.json\",\n  \"title\": \"KmsEncryptionConfig\",\n  \"type\": \"object\",\n  \"required\": [\n    \"CmkType\"\n  ],\n  \"properties\": {\n    \"CmkType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmkType\"\n        },\n        {\n          \"description\": \" The type of customer-managed-key(CMK) used for encryption. The two types of supported CMKs are customer owned CMKs and AWS owned CMKs. \"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKeyID\"\n        },\n        {\n          \"description\": \" The KMS encryption key id/alias used to encrypt the data store contents at rest. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" The\
  \ customer-managed-key(CMK) used when creating a data store. If a customer owned key is not specified, an AWS owned key will be used for encryption. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-kms-encryption-config-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: KmsEncryptionConfig
---
