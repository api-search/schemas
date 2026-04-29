---
description: Settings for decrypting any input files that you encrypt before you upload them to Amazon S3. MediaConvert can decrypt files only when you use AWS Key Management Service (KMS) to encrypt the data key that you use to encrypt your content.
layout: schema
name: InputDecryptionSettings
properties_list:
- description: ''
  name: DecryptionMode
  type: object
- description: ''
  name: EncryptedDecryptionKey
  type: object
- description: ''
  name: InitializationVector
  type: object
- description: ''
  name: KmsKeyRegion
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-input-decryption-settings-schema.json
slug: mediaconvert-api-input-decryption-settings
source_filename: mediaconvert-api-input-decryption-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-decryption-settings-schema.json\",\n  \"title\": \"InputDecryptionSettings\",\n  \"description\": \"Settings for decrypting any input files that you encrypt before you upload them to Amazon S3. MediaConvert can decrypt files only when you use AWS Key Management Service (KMS) to encrypt the data key that you use to encrypt your content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DecryptionMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecryptionMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"decryptionMode\"\n          },\n          \"description\": \"Specify the encryption mode that you used to encrypt your input files.\"\n        }\n      ]\n    },\n    \"EncryptedDecryptionKey\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin24Max512PatternAZaZ0902\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptedDecryptionKey\"\n          },\n          \"description\": \"Warning! Don't provide your encryption key in plaintext. Your job settings could be intercepted, making your encrypted content vulnerable. Specify the encrypted version of the data key that you used to encrypt your content. The data key must be encrypted by AWS Key Management Service (KMS). The key can be 128, 192, or 256 bits.\"\n        }\n      ]\n    },\n    \"InitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin16Max24PatternAZaZ0922AZaZ0916\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"initializationVector\"\n          },\n          \"description\": \"Specify the initialization vector that you used when you encrypted your content before uploading it to Amazon S3. You\
  \ can use a 16-byte initialization vector with any encryption mode. Or, you can use a 12-byte initialization vector with GCM or CTR. MediaConvert accepts only initialization vectors that are base64-encoded.\"\n        }\n      ]\n    },\n    \"KmsKeyRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin9Max19PatternAZ26EastWestCentralNorthSouthEastWest1912\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsKeyRegion\"\n          },\n          \"description\": \"Specify the AWS Region for AWS Key Management Service (KMS) that you used to encrypt your data key, if that Region is different from the one you are using for AWS Elemental MediaConvert.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-decryption-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputDecryptionSettings
---
