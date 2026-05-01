---
description: <p>Includes encryption-related information, such as the AWS KMS key used for encrypting data at rest and whether you want MSK to encrypt your data in transit.</p>
layout: schema
name: EncryptionInfo
properties_list:
- description: ''
  name: EncryptionAtRest
  type: object
- description: ''
  name: EncryptionInTransit
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-encryption-info-schema.json
slug: msk-api-encryption-info
source_filename: msk-api-encryption-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-encryption-info-schema.json\",\n  \"title\": \"EncryptionInfo\",\n  \"description\": \"\\n            <p>Includes encryption-related information, such as the AWS KMS key used for encrypting data at rest and whether you want MSK to encrypt your data in transit.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncryptionAtRest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionAtRest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionAtRest\"\n          },\n          \"description\": \"\\n            <p>The data-volume encryption details.</p>\"\n        }\n      ]\n    },\n    \"EncryptionInTransit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionInTransit\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"encryptionInTransit\"\n          },\n          \"description\": \"\\n            <p>The details for encryption in transit.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-encryption-info-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EncryptionInfo
---
