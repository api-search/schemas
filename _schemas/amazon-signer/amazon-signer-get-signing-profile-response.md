---
description: GetSigningProfileResponse schema from AWS Signer API
layout: schema
name: GetSigningProfileResponse
properties_list:
- description: ''
  name: profileName
  type: object
- description: ''
  name: profileVersion
  type: object
- description: ''
  name: profileVersionArn
  type: object
- description: Revocation information for a signing profile.
  name: revocationRecord
  type: object
- description: ''
  name: signingMaterial
  type: object
- description: ''
  name: platformId
  type: object
- description: ''
  name: platformDisplayName
  type: object
- description: The validity period for a signing job.
  name: signatureValidityPeriod
  type: object
- description: ''
  name: overrides
  type: object
- description: ''
  name: signingParameters
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-get-signing-profile-response-schema.json
slug: amazon-signer-get-signing-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-get-signing-profile-response-schema.json\",\n  \"title\": \"GetSigningProfileResponse\",\n  \"description\": \"GetSigningProfileResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9_]{2,}\",\n          \"minLength\": 2,\n          \"maxLength\": 64\n        },\n        {\n          \"description\": \"The name of the target signing profile.\"\n        }\n      ]\n    },\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The current version of\
  \ the signing profile.\"\n        }\n      ]\n    },\n    \"profileVersionArn\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"minLength\": 20,\n          \"maxLength\": 2048\n        },\n        {\n          \"description\": \"The signing profile ARN, including the profile version.\"\n        }\n      ]\n    },\n    \"revocationRecord\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"revocationEffectiveFrom\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Timestamp\"\n            },\n            {\n              \"description\": \"The time when revocation becomes effective.\"\n            }\n          ]\n        },\n        \"revokedAt\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Timestamp\"\n            },\n            {\n              \"description\": \"The time when the signing profile was revoked.\"\n            }\n          ]\n        },\n\
  \        \"revokedBy\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/String\"\n            },\n            {\n              \"description\": \"The identity of the revoker.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Revocation information for a signing profile.\"\n    },\n    \"signingMaterial\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"certificateArn\"\n          ],\n          \"properties\": {\n            \"certificateArn\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/CertificateArn\"\n                },\n                {\n                  \"description\": \"The Amazon Resource Name (ARN) of the certificates that is used to sign your code.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The ACM certificate that is used to sign your code.\"\
  \n        },\n        {\n          \"description\": \"The ARN of the certificate that the target profile uses for signing operations.\"\n        }\n      ]\n    },\n    \"platformId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of the platform that is used by the target signing profile.\"\n        }\n      ]\n    },\n    \"platformDisplayName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A human-readable name for the signing platform associated with the signing profile.\"\n        }\n      ]\n    },\n    \"signatureValidityPeriod\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Integer\"\n            },\n            {\n              \"description\": \"The numerical value of the time unit for signature validity.\"\n\
  \            }\n          ]\n        },\n        \"type\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ValidityType\"\n            },\n            {\n              \"description\": \"The time unit for signature validity.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"The validity period for a signing job.\"\n    },\n    \"overrides\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"signingConfiguration\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/SigningConfigurationOverrides\"\n                },\n                {\n                  \"description\": \"A signing configuration that overrides the default encryption or hash algorithm of a signing job.\"\n                }\n              ]\n            },\n            \"signingImageFormat\": {\n              \"allOf\": [\n                {\n    \
  \              \"$ref\": \"#/components/schemas/ImageFormat\"\n                },\n                {\n                  \"description\": \"A signed image is a JSON object. When overriding the default signing platform configuration, a customer can select either of two signing formats, <code>JSONEmbedded</code> or <code>JSONDetached</code>. (A third format value, <code>JSON</code>, is reserved for future use.) With <code>JSONEmbedded</code>, the signing image has the payload embedded in it. With <code>JSONDetached</code>, the payload is not be embedded in the signing image.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Any overrides that are applied to the signing configuration of a code signing platform.\"\n        },\n        {\n          \"description\": \"A list of overrides applied by the target signing profile for signing operations.\"\n        }\n      ]\n    },\n    \"signingParameters\": {\n      \"allOf\": [\n        {\n      \
  \    \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/SigningParameterValue\"\n          }\n        },\n        {\n          \"description\": \"A map of key-value pairs for signing operations that is attached to the target signing profile.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Active\",\n            \"Canceled\",\n            \"Revoked\"\n          ]\n        },\n        {\n          \"description\": \"The status of the target signing profile.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Reason for the status of the target signing profile.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\"\
  : \"The Amazon Resource Name (ARN) for the signing profile.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"minProperties\": 1,\n          \"maxProperties\": 200,\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          }\n        },\n        {\n          \"description\": \"A list of tags associated with the signing profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-get-signing-profile-response-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: GetSigningProfileResponse
---
