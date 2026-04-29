---
description: Contains information about the signing configurations and parameters that are used to perform a code signing job.
layout: schema
name: SigningPlatform
properties_list:
- description: ''
  name: platformId
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: partner
  type: object
- description: ''
  name: target
  type: object
- description: ''
  name: category
  type: object
- description: ''
  name: signingConfiguration
  type: object
- description: The image format of a code signing platform or profile.
  name: signingImageFormat
  type: object
- description: ''
  name: maxSizeInMB
  type: object
- description: ''
  name: revocationSupported
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-platform-schema.json
slug: amazon-signer-signing-platform
source_filename: amazon-signer-signing-platform-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-platform-schema.json\",\n  \"title\": \"SigningPlatform\",\n  \"description\": \"Contains information about the signing configurations and parameters that are used to perform a code signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platformId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of a code signing platform.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The display name of a code signing platform.\"\n        }\n      ]\n    },\n    \"partner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\"\
  : \"Any partner entities linked to a code signing platform.\"\n        }\n      ]\n    },\n    \"target\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The types of targets that can be signed by a code signing platform.\"\n        }\n      ]\n    },\n    \"category\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"AWSIoT\"\n          ]\n        },\n        {\n          \"description\": \"The category of a code signing platform.\"\n        }\n      ]\n    },\n    \"signingConfiguration\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"encryptionAlgorithmOptions\",\n            \"hashAlgorithmOptions\"\n          ],\n          \"properties\": {\n            \"encryptionAlgorithmOptions\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/EncryptionAlgorithmOptions\"\
  \n                },\n                {\n                  \"description\": \"The encryption algorithm options that are available for a code signing job.\"\n                }\n              ]\n            },\n            \"hashAlgorithmOptions\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/HashAlgorithmOptions\"\n                },\n                {\n                  \"description\": \"The hash algorithm options that are available for a code signing job.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The configuration of a code signing operation.\"\n        },\n        {\n          \"description\": \"The configuration of a code signing platform. This includes the designated hash algorithm and encryption algorithm of a signing platform.\"\n        }\n      ]\n    },\n    \"signingImageFormat\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"supportedFormats\",\n\
  \        \"defaultFormat\"\n      ],\n      \"properties\": {\n        \"supportedFormats\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ImageFormats\"\n            },\n            {\n              \"description\": \"The supported formats of a code signing image.\"\n            }\n          ]\n        },\n        \"defaultFormat\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ImageFormat\"\n            },\n            {\n              \"description\": \"The default format of a code signing image.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"The image format of a code signing platform or profile.\"\n    },\n    \"maxSizeInMB\": {\n      \"allOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"description\": \"The maximum size (in MB) of code that can be signed by a code signing platform.\"\n        }\n      ]\n    },\n    \"revocationSupported\"\
  : {\n      \"allOf\": [\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"description\": \"Indicates whether revocation is supported for the platform.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-platform-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningPlatform
---
