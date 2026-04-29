---
description: The encryption settings, if any, that are used for decrypting your input files or encrypting your output files. If your input file is encrypted, you must specify the mode that Elastic Transcoder uses to decrypt your file, otherwise you must specify the mode you want Elastic Transcoder to use to encrypt your output files.
layout: schema
name: Encryption
properties_list:
- description: ''
  name: Mode
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: KeyMd5
  type: object
- description: ''
  name: InitializationVector
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-encryption-schema.json
slug: amazon-elastic-transcoder-encryption
source_filename: amazon-elastic-transcoder-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-encryption-schema.json\",\n  \"title\": \"Encryption\",\n  \"description\": \"The encryption settings, if any, that are used for decrypting your input files or encrypting your output files. If your input file is encrypted, you must specify the mode that Elastic Transcoder uses to decrypt your file, otherwise you must specify the mode you want Elastic Transcoder to use to encrypt your output files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionMode\"\n        },\n        {\n          \"description\": \"<p>The specific server-side encryption mode that you want Elastic Transcoder to use when decrypting your input files or encrypting your output files. Elastic Transcoder\
  \ supports the following options:</p> <ul> <li> <p> <b>s3:</b> Amazon S3 creates and manages the keys used for encrypting your files.</p> </li> <li> <p> <b>s3-aws-kms:</b> Amazon S3 calls the Amazon Key Management Service, which creates and manages the keys that are used for encrypting your files. If you specify <code>s3-aws-kms</code> and you don't want to use the default key, you must add the AWS-KMS key that you want to use to your pipeline.</p> </li> <li> <p> <b>aes-cbc-pkcs7:</b> A padded cipher-block mode of operation originally used for HLS files.</p> </li> <li> <p> <b>aes-ctr:</b> AES Counter Mode.</p> </li> <li> <p> <b>aes-gcm:</b> AES Galois Counter Mode, a mode of operation that is an authenticated encryption format, meaning that a file, key, or initialization vector that has been tampered with fails the decryption process.</p> </li> </ul> <p>For all three AES options, you must provide the following settings, which must be base64-encoded:</p> <ul> <li> <p> <b>Key</b> </p> </li>\
  \ <li> <p> <b>Key MD5</b> </p> </li> <li> <p> <b>Initialization Vector</b> </p> </li> </ul> <important> <p>For the AES modes, your private encryption keys and your unencrypted data are never stored by AWS; therefore, it is important that you safely manage your encryption keys. If you lose them, you won't be able to unencrypt your data.</p> </important>\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Base64EncodedString\"\n        },\n        {\n          \"description\": \"<p>The data encryption key that you want Elastic Transcoder to use to encrypt your output file, or that was used to encrypt your input file. The key must be base64-encoded and it must be one of the following bit lengths before being base64-encoded:</p> <p> <code>128</code>, <code>192</code>, or <code>256</code>. </p> <p>The key must also be encrypted by using the Amazon Key Management Service.</p>\"\n        }\n      ]\n    },\n    \"KeyMd5\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Base64EncodedString\"\n        },\n        {\n          \"description\": \"The MD5 digest of the key that you used to encrypt your input file, or that you want Elastic Transcoder to use to encrypt your output file. Elastic Transcoder uses the key digest as a checksum to make sure your key was not corrupted in transit. The key MD5 must be base64-encoded, and it must be exactly 16 bytes long before being base64-encoded.\"\n        }\n      ]\n    },\n    \"InitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeroTo255String\"\n        },\n        {\n          \"description\": \"The series of random bits created by a random bit generator, unique for every encryption operation, that you used to encrypt your input files or that you want Elastic Transcoder to use to encrypt your output files. The initialization vector must be base64-encoded, and it must be exactly 16 bytes\
  \ long before being base64-encoded.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-encryption-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Encryption
---
