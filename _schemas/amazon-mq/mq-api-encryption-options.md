---
description: <important><p>Does not apply to RabbitMQ brokers.</p></important> <p>Encryption options for the broker.</p>
layout: schema
name: EncryptionOptions
properties_list:
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: UseAwsOwnedKey
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-encryption-options-schema.json
slug: mq-api-encryption-options
source_filename: mq-api-encryption-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-encryption-options-schema.json\",\n  \"title\": \"EncryptionOptions\",\n  \"description\": \"<important><p>Does not apply to RabbitMQ brokers.</p></important> <p>Encryption options for the broker.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsKeyId\"\n          },\n          \"description\": \"The customer master key (CMK) to use for the AWS Key Management Service (KMS). This key is used to encrypt your data at rest. If not provided, Amazon MQ will use a default CMK to encrypt your data.\"\n        }\n      ]\n    },\n    \"UseAwsOwnedKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"useAwsOwnedKey\"\n          },\n          \"description\": \"Enables the use of an AWS owned CMK using AWS Key Management Service (KMS). Set to true by default, if no value is provided, for example, for RabbitMQ brokers.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UseAwsOwnedKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-encryption-options-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: EncryptionOptions
---
