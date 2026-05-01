---
description: A configuration for accessing an external Secure Packager and Encoder Key Exchange (SPEKE) service that will provide encryption keys.
layout: schema
name: SpekeKeyProvider
properties_list:
- description: ''
  name: CertificateArn
  type: object
- description: ''
  name: EncryptionContractConfiguration
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SystemIds
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-speke-key-provider-schema.json
slug: mediapackage-api-speke-key-provider
source_filename: mediapackage-api-speke-key-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-speke-key-provider-schema.json\",\n  \"title\": \"SpekeKeyProvider\",\n  \"description\": \"A configuration for accessing an external Secure Packager and Encoder Key Exchange (SPEKE) service that will provide encryption keys.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"certificateArn\"\n          },\n          \"description\": \"An Amazon Resource Name (ARN) of a Certificate Manager certificate\\nthat MediaPackage will use for enforcing secure end-to-end data\\ntransfer with the key provider service.\\n\"\n        }\n      ]\n    },\n    \"EncryptionContractConfiguration\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/EncryptionContractConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionContractConfiguration\"\n          }\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceId\"\n          },\n          \"description\": \"The resource ID to include in key requests.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"An Amazon Resource Name (ARN) of an IAM role that AWS Elemental\\nMediaPackage will assume when accessing the key provider service.\\n\"\n        }\n      ]\n    },\n    \"SystemIds\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"systemIds\"\n          },\n          \"description\": \"The system IDs to include in key requests.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"The URL of the external key provider service.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceId\",\n    \"SystemIds\",\n    \"Url\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-speke-key-provider-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SpekeKeyProvider
---
