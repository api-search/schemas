---
description: Information about the encryption of the flow.
layout: schema
name: UpdateEncryption
properties_list:
- description: ''
  name: Algorithm
  type: object
- description: ''
  name: ConstantInitializationVector
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: KeyType
  type: object
- description: ''
  name: Region
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SecretArn
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-update-encryption-schema.json
slug: mediaconnect-api-update-encryption
source_filename: mediaconnect-api-update-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-encryption-schema.json\",\n  \"title\": \"UpdateEncryption\",\n  \"description\": \"Information about the encryption of the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Algorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Algorithm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"algorithm\"\n          },\n          \"description\": \"The type of algorithm that is used for the encryption (such as aes128, aes192, or aes256).\"\n        }\n      ]\n    },\n    \"ConstantInitializationVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"constantInitializationVector\"\n          },\n      \
  \    \"description\": \"A 128-bit, 16-byte hex value represented by a 32-character string, to be used with the key for encrypting content. This parameter is not valid for static key encryption.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deviceId\"\n          },\n          \"description\": \"The value of one of the devices that you configured with your digital rights management (DRM) platform key provider. This parameter is required for SPEKE encryption and is not valid for static key encryption.\"\n        }\n      ]\n    },\n    \"KeyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyType\"\n          },\n          \"description\": \"The type of key that is used for the encryption. If no keyType is provided,\
  \ the service will use the default setting (static-key).\"\n        }\n      ]\n    },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"region\"\n          },\n          \"description\": \"The AWS Region that the API Gateway proxy endpoint was created in. This parameter is required for SPEKE encryption and is not valid for static key encryption.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceId\"\n          },\n          \"description\": \"An identifier for the content. The service sends this value to the key server to identify the current endpoint. The resource ID is also known as the content ID. This parameter is required for SPEKE encryption and is not valid for static key encryption.\"\n   \
  \     }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"The ARN of the role that you created during setup (when you set up AWS Elemental MediaConnect as a trusted entity).\"\n        }\n      ]\n    },\n    \"SecretArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"secretArn\"\n          },\n          \"description\": \"The ARN of the secret that you created in AWS Secrets Manager to store the encryption key. This parameter is required for static key encryption and is not valid for SPEKE encryption.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n   \
  \         \"name\": \"url\"\n          },\n          \"description\": \"The URL from the API Gateway proxy that you set up to talk to your key server. This parameter is required for SPEKE encryption and is not valid for static key encryption.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-update-encryption-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: UpdateEncryption
---
