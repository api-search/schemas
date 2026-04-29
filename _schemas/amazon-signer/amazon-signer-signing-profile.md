---
description: Contains information about the ACM certificates and code signing configuration parameters that can be used by a given code signing user.
layout: schema
name: SigningProfile
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
  name: platformDisplayName
  type: object
- description: ''
  name: signingParameters
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-profile-schema.json
slug: amazon-signer-signing-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-profile-schema.json\",\n  \"title\": \"SigningProfile\",\n  \"description\": \"Contains information about the ACM certificates and code signing configuration parameters that can be used by a given code signing user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9_]{2,}\",\n          \"minLength\": 2,\n          \"maxLength\": 64\n        },\n        {\n          \"description\": \"The name of the signing profile.\"\n        }\n      ]\n    },\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n\
  \          \"description\": \"The version of a signing profile.\"\n        }\n      ]\n    },\n    \"profileVersionArn\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"minLength\": 20,\n          \"maxLength\": 2048\n        },\n        {\n          \"description\": \"The ARN of a signing profile, including the profile version.\"\n        }\n      ]\n    },\n    \"signingMaterial\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"certificateArn\"\n          ],\n          \"properties\": {\n            \"certificateArn\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/CertificateArn\"\n                },\n                {\n                  \"description\": \"The Amazon Resource Name (ARN) of the certificates that is used to sign your code.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The ACM\
  \ certificate that is used to sign your code.\"\n        },\n        {\n          \"description\": \"The ACM certificate that is available for use by a signing profile.\"\n        }\n      ]\n    },\n    \"signatureValidityPeriod\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/Integer\"\n                },\n                {\n                  \"description\": \"The numerical value of the time unit for signature validity.\"\n                }\n              ]\n            },\n            \"type\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/ValidityType\"\n                },\n                {\n                  \"description\": \"The time unit for signature validity.\"\n                }\n              ]\n            }\n          },\n          \"description\"\
  : \"The validity period for a signing job.\"\n        },\n        {\n          \"description\": \"The validity period for a signing job created using this signing profile.\"\n        }\n      ]\n    },\n    \"platformId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of a platform that is available for use by a signing profile.\"\n        }\n      ]\n    },\n    \"platformDisplayName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The name of the signing platform.\"\n        }\n      ]\n    },\n    \"signingParameters\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/SigningParameterValue\"\n          }\n        },\n        {\n          \"description\": \"The parameters that are available for use by a code signing user.\"\n        }\n\
  \      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Active\",\n            \"Canceled\",\n            \"Revoked\"\n          ]\n        },\n        {\n          \"description\": \"The status of a code signing profile.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the signing profile.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"minProperties\": 1,\n          \"maxProperties\": 200,\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          }\n        },\n        {\n          \"description\": \"A list of tags associated with the signing profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-profile-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningProfile
---
