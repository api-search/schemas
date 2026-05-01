---
description: The HLS content protection settings, if any, that you want Elastic Transcoder to apply to your output files.
layout: schema
name: HlsContentProtection
properties_list:
- description: ''
  name: Method
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
- description: ''
  name: LicenseAcquisitionUrl
  type: object
- description: ''
  name: KeyStoragePolicy
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-hls-content-protection-schema.json
slug: amazon-elastic-transcoder-hls-content-protection
source_filename: amazon-elastic-transcoder-hls-content-protection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-hls-content-protection-schema.json\",\n  \"title\": \"HlsContentProtection\",\n  \"description\": \"The HLS content protection settings, if any, that you want Elastic Transcoder to apply to your output files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Method\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsContentProtectionMethod\"\n        },\n        {\n          \"description\": \"<p>The content protection method for your output. The only valid value is: <code>aes-128</code>.</p> <p>This value is written into the method attribute of the <code>EXT-X-KEY</code> metadata tag in the output playlist.</p>\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Base64EncodedString\"\
  \n        },\n        {\n          \"description\": \"<p>If you want Elastic Transcoder to generate a key for you, leave this field blank.</p> <p>If you choose to supply your own key, you must encrypt the key by using AWS KMS. The key must be base64-encoded, and it must be one of the following bit lengths before being base64-encoded:</p> <p> <code>128</code>, <code>192</code>, or <code>256</code>. </p>\"\n        }\n      ]\n    },\n    \"KeyMd5\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Base64EncodedString\"\n        },\n        {\n          \"description\": \"<p>If Elastic Transcoder is generating your key for you, you must leave this field blank.</p> <p>The MD5 digest of the key that you want Elastic Transcoder to use to encrypt your output file, and that you want Elastic Transcoder to use as a checksum to make sure your key was not corrupted in transit. The key MD5 must be base64-encoded, and it must be exactly 16 bytes before being base64- encoded.</p>\"\
  \n        }\n      ]\n    },\n    \"InitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeroTo255String\"\n        },\n        {\n          \"description\": \"<p>If Elastic Transcoder is generating your key for you, you must leave this field blank.</p> <p>The series of random bits created by a random bit generator, unique for every encryption operation, that you want Elastic Transcoder to use to encrypt your output files. The initialization vector must be base64-encoded, and it must be exactly 16 bytes before being base64-encoded.</p>\"\n        }\n      ]\n    },\n    \"LicenseAcquisitionUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeroTo512String\"\n        },\n        {\n          \"description\": \"The location of the license key required to decrypt your HLS playlist. The URL must be an absolute path, and is referenced in the URI attribute of the EXT-X-KEY metadata tag in the playlist file.\"\n\
  \        }\n      ]\n    },\n    \"KeyStoragePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyStoragePolicy\"\n        },\n        {\n          \"description\": \"Specify whether you want Elastic Transcoder to write your HLS license key to an Amazon S3 bucket. If you choose <code>WithVariantPlaylists</code>, <code>LicenseAcquisitionUrl</code> must be left blank and Elastic Transcoder writes your data key into the same bucket as the associated playlist.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-hls-content-protection-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: HlsContentProtection
---
