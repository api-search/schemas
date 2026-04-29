---
description: PutSigningProfileRequest schema from AWS Signer API
layout: schema
name: PutSigningProfileRequest
properties_list:
- description: ''
  name: signingMaterial
  type: object
- description: ''
  name: signatureValidityPeriod
  type: object
- description: ''
  name: platformId
  type: object
- description: ''
  name: overrides
  type: object
- description: ''
  name: signingParameters
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-put-signing-profile-request-schema.json
slug: amazon-signer-put-signing-profile-request
source_filename: amazon-signer-put-signing-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-put-signing-profile-request-schema.json\",\n  \"title\": \"PutSigningProfileRequest\",\n  \"description\": \"PutSigningProfileRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"signingMaterial\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"certificateArn\"\n          ],\n          \"properties\": {\n            \"certificateArn\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/CertificateArn\"\n                },\n                {\n                  \"description\": \"The Amazon Resource Name (ARN) of the certificates that is used to sign your code.\"\n                }\n              ]\n            }\n          },\n          \"description\"\
  : \"The ACM certificate that is used to sign your code.\"\n        },\n        {\n          \"description\": \"The AWS Certificate Manager certificate that will be used to sign code with the new signing profile.\"\n        }\n      ]\n    },\n    \"signatureValidityPeriod\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/Integer\"\n                },\n                {\n                  \"description\": \"The numerical value of the time unit for signature validity.\"\n                }\n              ]\n            },\n            \"type\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/ValidityType\"\n                },\n                {\n                  \"description\": \"The time unit for signature validity.\"\n                }\n              ]\n        \
  \    }\n          },\n          \"description\": \"The validity period for a signing job.\"\n        },\n        {\n          \"description\": \"The default validity period override for any signature generated using this signing profile. If unspecified, the default is 135 months.\"\n        }\n      ]\n    },\n    \"platformId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of the signing platform to be created.\"\n        }\n      ]\n    },\n    \"overrides\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"signingConfiguration\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/SigningConfigurationOverrides\"\n                },\n                {\n                  \"description\": \"A signing configuration that overrides the default encryption or hash algorithm of a signing job.\"\n        \
  \        }\n              ]\n            },\n            \"signingImageFormat\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/ImageFormat\"\n                },\n                {\n                  \"description\": \"A signed image is a JSON object. When overriding the default signing platform configuration, a customer can select either of two signing formats, <code>JSONEmbedded</code> or <code>JSONDetached</code>. (A third format value, <code>JSON</code>, is reserved for future use.) With <code>JSONEmbedded</code>, the signing image has the payload embedded in it. With <code>JSONDetached</code>, the payload is not be embedded in the signing image.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Any overrides that are applied to the signing configuration of a code signing platform.\"\n        },\n        {\n          \"description\": \"A subfield of <code>platform</code>. This specifies\
  \ any different configuration options that you want to apply to the chosen platform (such as a different <code>hash-algorithm</code> or <code>signing-algorithm</code>).\"\n        }\n      ]\n    },\n    \"signingParameters\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/SigningParameterValue\"\n          }\n        },\n        {\n          \"description\": \"Map of key-value pairs for signing. These can include any information that you want to use during signing.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"minProperties\": 1,\n          \"maxProperties\": 200,\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          }\n        },\n        {\n          \"description\": \"Tags to be associated with the signing profile that is being created.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"platformId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-put-signing-profile-request-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: PutSigningProfileRequest
---
