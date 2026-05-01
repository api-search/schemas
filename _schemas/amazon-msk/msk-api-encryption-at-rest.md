---
description: <p>The data-volume encryption details.</p>
layout: schema
name: EncryptionAtRest
properties_list:
- description: ''
  name: DataVolumeKMSKeyId
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-encryption-at-rest-schema.json
slug: msk-api-encryption-at-rest
source_filename: msk-api-encryption-at-rest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-encryption-at-rest-schema.json\",\n  \"title\": \"EncryptionAtRest\",\n  \"description\": \"\\n            <p>The data-volume encryption details.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DataVolumeKMSKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataVolumeKMSKeyId\"\n          },\n          \"description\": \"\\n            <p>The ARN of the AWS KMS key for encrypting data at rest. If you don't specify a KMS key, MSK creates one for you and uses it.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DataVolumeKMSKeyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-encryption-at-rest-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EncryptionAtRest
---
