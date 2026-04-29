---
description: Settings for how your job outputs are encrypted as they are uploaded to Amazon S3.
layout: schema
name: S3EncryptionSettings
properties_list:
- description: ''
  name: EncryptionType
  type: object
- description: ''
  name: KmsEncryptionContext
  type: object
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-s3-encryption-settings-schema.json
slug: mediaconvert-api-s3-encryption-settings
source_filename: mediaconvert-api-s3-encryption-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-s3-encryption-settings-schema.json\",\n  \"title\": \"S3EncryptionSettings\",\n  \"description\": \"Settings for how your job outputs are encrypted as they are uploaded to Amazon S3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ServerSideEncryptionType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionType\"\n          },\n          \"description\": \"Specify how you want your data keys managed. AWS uses data keys to encrypt your content. AWS also encrypts the data keys themselves, using a customer master key (CMK), and then stores the encrypted data keys alongside your encrypted content. Use this setting to specify which AWS service manages the\
  \ CMK. For simplest set up, choose Amazon S3 (SERVER_SIDE_ENCRYPTION_S3). If you want your master key to be managed by AWS Key Management Service (KMS), choose AWS KMS (SERVER_SIDE_ENCRYPTION_KMS). By default, when you choose AWS KMS, KMS uses the AWS managed customer master key (CMK) associated with Amazon S3 to encrypt your data keys. You can optionally choose to specify a different, customer managed CMK. Do so by specifying the Amazon Resource Name (ARN) of the key for the setting KMS ARN (kmsKeyArn).\"\n        }\n      ]\n    },\n    \"KmsEncryptionContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternAZaZ0902\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsEncryptionContext\"\n          },\n          \"description\": \"Optionally, specify the encryption context that you want to use alongside your KMS key. AWS KMS uses this encryption context as additional authenticated data (AAD) to support authenticated\
  \ encryption. This value must be a base64-encoded UTF-8 string holding JSON which represents a string-string map. To use this setting, you must also set Server-side encryption (S3ServerSideEncryptionType) to AWS KMS (SERVER_SIDE_ENCRYPTION_KMS). For more information about encryption context, see: https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternArnAwsUsGovCnKmsAZ26EastWestCentralNorthSouthEastWest1912D12KeyAFAF098AFAF094AFAF094AFAF094AFAF0912MrkAFAF0932\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsKeyArn\"\n          },\n          \"description\": \"Optionally, specify the customer master key (CMK) that you want to use to encrypt the data key that AWS uses to encrypt your output content. Enter the Amazon Resource Name (ARN) of the CMK. To use this setting, you must also set Server-side\
  \ encryption (S3ServerSideEncryptionType) to AWS KMS (SERVER_SIDE_ENCRYPTION_KMS). If you set Server-side encryption to AWS KMS but don't specify a CMK here, AWS uses the AWS managed CMK associated with Amazon S3.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-s3-encryption-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: S3EncryptionSettings
---
