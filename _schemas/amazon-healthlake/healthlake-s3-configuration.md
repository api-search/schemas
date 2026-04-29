---
description: The configuration of the S3 bucket for either an import or export job. This includes assigning permissions for access.
layout: schema
name: S3Configuration
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: KmsKeyId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-s3-configuration-schema.json
slug: healthlake-s3-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-s3-configuration-schema.json\",\n  \"title\": \"S3Configuration\",\n  \"type\": \"object\",\n  \"required\": [\n    \"S3Uri\",\n    \"KmsKeyId\"\n  ],\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \" The S3Uri is the user specified S3 location of the FHIR data to be imported into AWS HealthLake. \"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionKeyID\"\n        },\n        {\n          \"description\": \" The KMS key ID used to access the S3 bucket. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" The configuration of the S3 bucket for either an import or export job. This\
  \ includes assigning permissions for access. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-s3-configuration-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: S3Configuration
---
