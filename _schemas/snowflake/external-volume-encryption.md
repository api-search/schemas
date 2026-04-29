---
description: ''
layout: schema
name: Encryption
properties_list:
- description: Specifies the encryption type used.
  name: type
  type: string
- description: Specifies the ID for the Cloud KMS-managed key used to encrypt files written to the bucket.
  name: kms_key_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/external-volume-encryption-schema.json
slug: external-volume-encryption
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Encryption\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the encryption type used.\"\n    },\n    \"kms_key_id\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the ID for the Cloud KMS-managed key used to encrypt files written to the bucket.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/external-volume-encryption-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Encryption
---
