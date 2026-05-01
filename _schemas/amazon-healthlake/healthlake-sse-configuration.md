---
description: The server-side encryption key configuration for a customer provided encryption key.
layout: schema
name: SseConfiguration
properties_list:
- description: ''
  name: KmsEncryptionConfig
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-sse-configuration-schema.json
slug: healthlake-sse-configuration
source_filename: healthlake-sse-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-sse-configuration-schema.json\",\n  \"title\": \"SseConfiguration\",\n  \"type\": \"object\",\n  \"required\": [\n    \"KmsEncryptionConfig\"\n  ],\n  \"properties\": {\n    \"KmsEncryptionConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsEncryptionConfig\"\n        },\n        {\n          \"description\": \" The KMS encryption configuration used to provide details for data encryption. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" The server-side encryption key configuration for a customer provided encryption key. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-sse-configuration-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: SseConfiguration
---
