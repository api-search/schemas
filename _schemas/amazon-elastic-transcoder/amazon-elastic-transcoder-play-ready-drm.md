---
description: <p>The PlayReady DRM settings, if any, that you want Elastic Transcoder to apply to the output files associated with this playlist.</p> <p>PlayReady DRM encrypts your media files using <code>aes-ctr</code> encryption.</p> <p>If you use DRM for an <code>HLSv3</code> playlist, your outputs must have a master playlist.</p>
layout: schema
name: PlayReadyDrm
properties_list:
- description: ''
  name: Format
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: KeyMd5
  type: object
- description: ''
  name: KeyId
  type: object
- description: ''
  name: InitializationVector
  type: object
- description: ''
  name: LicenseAcquisitionUrl
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-play-ready-drm-schema.json
slug: amazon-elastic-transcoder-play-ready-drm
source_filename: amazon-elastic-transcoder-play-ready-drm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-play-ready-drm-schema.json\",\n  \"title\": \"PlayReadyDrm\",\n  \"description\": \"<p>The PlayReady DRM settings, if any, that you want Elastic Transcoder to apply to the output files associated with this playlist.</p> <p>PlayReady DRM encrypts your media files using <code>aes-ctr</code> encryption.</p> <p>If you use DRM for an <code>HLSv3</code> playlist, your outputs must have a master playlist.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlayReadyDrmFormatString\"\n        },\n        {\n          \"description\": \"The type of DRM, if any, that you want Elastic Transcoder to apply to the output files associated with this playlist.\"\n        }\n      ]\n    },\n\
  \    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyBase64EncodedString\"\n        },\n        {\n          \"description\": \"<p>The DRM key for your file, provided by your DRM license provider. The key must be base64-encoded, and it must be one of the following bit lengths before being base64-encoded:</p> <p> <code>128</code>, <code>192</code>, or <code>256</code>. </p> <p>The key must also be encrypted by using AWS KMS.</p>\"\n        }\n      ]\n    },\n    \"KeyMd5\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyBase64EncodedString\"\n        },\n        {\n          \"description\": \"The MD5 digest of the key used for DRM on your file, and that you want Elastic Transcoder to use as a checksum to make sure your key was not corrupted in transit. The key MD5 must be base64-encoded, and it must be exactly 16 bytes before being base64-encoded.\"\n        }\n      ]\n    },\n    \"KeyId\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyIdGuid\"\n        },\n        {\n          \"description\": \"<p>The ID for your DRM key, so that your DRM license provider knows which key to provide.</p> <p>The key ID must be provided in big endian, and Elastic Transcoder converts it to little endian before inserting it into the PlayReady DRM headers. If you are unsure whether your license server provides your key ID in big or little endian, check with your DRM provider.</p>\"\n        }\n      ]\n    },\n    \"InitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZeroTo255String\"\n        },\n        {\n          \"description\": \"The series of random bits created by a random bit generator, unique for every encryption operation, that you want Elastic Transcoder to use to encrypt your files. The initialization vector must be base64-encoded, and it must be exactly 8 bytes long before being base64-encoded. If no initialization\
  \ vector is provided, Elastic Transcoder generates one for you.\"\n        }\n      ]\n    },\n    \"LicenseAcquisitionUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OneTo512String\"\n        },\n        {\n          \"description\": \"The location of the license key required to play DRM content. The URL must be an absolute path, and is referenced by the PlayReady header. The PlayReady header is referenced in the protection header of the client manifest for Smooth Streaming outputs, and in the EXT-X-DXDRM and EXT-XDXDRMINFO metadata tags for HLS playlist outputs. An example URL looks like this: <code>https://www.example.com/exampleKey/</code> \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-play-ready-drm-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: PlayReadyDrm
---
