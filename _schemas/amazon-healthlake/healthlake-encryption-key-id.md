---
description: ''
layout: schema
name: EncryptionKeyID
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-encryption-key-id-schema.json
slug: healthlake-encryption-key-id
source_filename: healthlake-encryption-key-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-encryption-key-id-schema.json\",\n  \"title\": \"EncryptionKeyID\",\n  \"type\": \"string\",\n  \"pattern\": \"(arn:aws((-us-gov)|(-iso)|(-iso-b)|(-cn))?:kms:)?([a-z]{2}-[a-z]+(-[a-z]+)?-\\\\d:)?(\\\\d{12}:)?(((key/)?[a-zA-Z0-9-_]+)|(alias/[a-zA-Z0-9:/_-]+))\",\n  \"minLength\": 1,\n  \"maxLength\": 400\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-encryption-key-id-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: EncryptionKeyID
---
