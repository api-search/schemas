---
description: DescribeSigningJobResponse schema from AWS Signer API
layout: schema
name: DescribeSigningJobResponse
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: source
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
- description: ''
  name: profileName
  type: object
- description: ''
  name: profileVersion
  type: object
- description: ''
  name: overrides
  type: object
- description: ''
  name: signingParameters
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: completedAt
  type: object
- description: ''
  name: signatureExpiresAt
  type: object
- description: ''
  name: requestedBy
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
- description: ''
  name: revocationRecord
  type: object
- description: ''
  name: signedObject
  type: object
- description: ''
  name: jobOwner
  type: object
- description: ''
  name: jobInvoker
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-describe-signing-job-response-schema.json
slug: amazon-signer-describe-signing-job-response
source_filename: amazon-signer-describe-signing-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-describe-signing-job-response-schema.json\",\n  \"title\": \"DescribeSigningJobResponse\",\n  \"description\": \"DescribeSigningJobResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of the signing job on output.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"s3\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/S3Source\"\n                },\n                {\n                  \"description\": \"The <code>S3Source</code> object.\"\n                }\n     \
  \         ]\n            }\n          },\n          \"description\": \"An <code>S3Source</code> object that contains information about the S3 bucket where you saved your unsigned code.\"\n        },\n        {\n          \"description\": \"The object that contains the name of your S3 bucket or your raw code.\"\n        }\n      ]\n    },\n    \"signingMaterial\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"certificateArn\"\n          ],\n          \"properties\": {\n            \"certificateArn\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/CertificateArn\"\n                },\n                {\n                  \"description\": \"The Amazon Resource Name (ARN) of the certificates that is used to sign your code.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The ACM certificate that is used to sign your code.\"\n  \
  \      },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of your code signing certificate.\"\n        }\n      ]\n    },\n    \"platformId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The microcontroller platform to which your signed code image will be distributed.\"\n        }\n      ]\n    },\n    \"platformDisplayName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A human-readable name for the signing platform associated with the signing job.\"\n        }\n      ]\n    },\n    \"profileName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9_]{2,}\",\n          \"minLength\": 2,\n          \"maxLength\": 64\n        },\n        {\n          \"description\": \"The name of the profile that initiated the signing operation.\"\n        }\n      ]\n    },\n    \"\
  profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The version of the signing profile used to initiate the signing job.\"\n        }\n      ]\n    },\n    \"overrides\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"signingConfiguration\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/SigningConfigurationOverrides\"\n                },\n                {\n                  \"description\": \"A signing configuration that overrides the default encryption or hash algorithm of a signing job.\"\n                }\n              ]\n            },\n            \"signingImageFormat\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/ImageFormat\"\
  \n                },\n                {\n                  \"description\": \"A signed image is a JSON object. When overriding the default signing platform configuration, a customer can select either of two signing formats, <code>JSONEmbedded</code> or <code>JSONDetached</code>. (A third format value, <code>JSON</code>, is reserved for future use.) With <code>JSONEmbedded</code>, the signing image has the payload embedded in it. With <code>JSONDetached</code>, the payload is not be embedded in the signing image.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Any overrides that are applied to the signing configuration of a code signing platform.\"\n        },\n        {\n          \"description\": \"A list of any overrides that were applied to the signing operation.\"\n        }\n      ]\n    },\n    \"signingParameters\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n         \
  \   \"$ref\": \"#/components/schemas/SigningParameterValue\"\n          }\n        },\n        {\n          \"description\": \"Map of user-assigned key-value pairs used during signing. These values contain any information that you specified for use in your signing job. \"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"Date and time that the signing job was created.\"\n        }\n      ]\n    },\n    \"completedAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"Date and time that the signing job was completed.\"\n        }\n      ]\n    },\n    \"signatureExpiresAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"Thr\
  \ expiration timestamp for the signature generated by the signing job.\"\n        }\n      ]\n    },\n    \"requestedBy\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The IAM principal that requested the signing job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"InProgress\",\n            \"Failed\",\n            \"Succeeded\"\n          ]\n        },\n        {\n          \"description\": \"Status of the signing job.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"String value that contains the status reason.\"\n        }\n      ]\n    },\n    \"revocationRecord\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"reason\": {\n \
  \             \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/String\"\n                },\n                {\n                  \"description\": \"A caller-supplied reason for revocation.\"\n                }\n              ]\n            },\n            \"revokedAt\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/Timestamp\"\n                },\n                {\n                  \"description\": \"The time of revocation.\"\n                }\n              ]\n            },\n            \"revokedBy\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/String\"\n                },\n                {\n                  \"description\": \"The identity of the revoker.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Revocation information for a signing job.\"\n        },\n        {\n          \"description\"\
  : \"A revocation record if the signature generated by the signing job has been revoked. Contains a timestamp and the ID of the IAM entity that revoked the signature.\"\n        }\n      ]\n    },\n    \"signedObject\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"s3\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/S3SignedObject\"\n                },\n                {\n                  \"description\": \"The <code>S3SignedObject</code>.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Points to an <code>S3SignedObject</code> object that contains information about your signed code image.\"\n        },\n        {\n          \"description\": \"Name of the S3 bucket where the signed code image is saved by code signing.\"\n        }\n      ]\n    },\n    \"jobOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"\
  string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the job owner.\"\n        }\n      ]\n    },\n    \"jobInvoker\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The IAM entity that initiated the signing job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-describe-signing-job-response-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: DescribeSigningJobResponse
---
