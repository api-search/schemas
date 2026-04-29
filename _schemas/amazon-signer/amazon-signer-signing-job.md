---
description: Contains information about a signing job.
layout: schema
name: SigningJob
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: signedObject
  type: object
- description: ''
  name: signingMaterial
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: isRevoked
  type: object
- description: ''
  name: profileName
  type: object
- description: ''
  name: profileVersion
  type: object
- description: ''
  name: platformId
  type: object
- description: ''
  name: platformDisplayName
  type: object
- description: ''
  name: signatureExpiresAt
  type: object
- description: ''
  name: jobOwner
  type: object
- description: ''
  name: jobInvoker
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-job-schema.json
slug: amazon-signer-signing-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-job-schema.json\",\n  \"title\": \"SigningJob\",\n  \"description\": \"Contains information about a signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of the signing job.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"s3\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/S3Source\"\n                },\n                {\n                  \"description\": \"The <code>S3Source</code> object.\"\n                }\n              ]\n            }\n          },\n          \"description\"\
  : \"An <code>S3Source</code> object that contains information about the S3 bucket where you saved your unsigned code.\"\n        },\n        {\n          \"description\": \"A <code>Source</code> that contains information about a signing job's code image source.\"\n        }\n      ]\n    },\n    \"signedObject\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"s3\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/S3SignedObject\"\n                },\n                {\n                  \"description\": \"The <code>S3SignedObject</code>.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Points to an <code>S3SignedObject</code> object that contains information about your signed code image.\"\n        },\n        {\n          \"description\": \"A <code>SignedObject</code> structure that contains information about a signing job's\
  \ signed code image.\"\n        }\n      ]\n    },\n    \"signingMaterial\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"certificateArn\"\n          ],\n          \"properties\": {\n            \"certificateArn\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/CertificateArn\"\n                },\n                {\n                  \"description\": \"The Amazon Resource Name (ARN) of the certificates that is used to sign your code.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The ACM certificate that is used to sign your code.\"\n        },\n        {\n          \"description\": \"A <code>SigningMaterial</code> object that contains the Amazon Resource Name (ARN) of the certificate used for the signing job.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\
  ,\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"The date and time that the signing job was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\n            \"InProgress\",\n            \"Failed\",\n            \"Succeeded\"\n          ]\n        },\n        {\n          \"description\": \"The status of the signing job.\"\n        }\n      ]\n    },\n    \"isRevoked\": {\n      \"allOf\": [\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the signing job is revoked.\"\n        }\n      ]\n    },\n    \"profileName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9_]{2,}\",\n          \"minLength\": 2,\n          \"maxLength\": 64\n        },\n        {\n          \"description\": \"The name of the signing profile that created a signing\
  \ job.\"\n        }\n      ]\n    },\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The version of the signing profile that created a signing job.\"\n        }\n      ]\n    },\n    \"platformId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The unique identifier for a signing platform.\"\n        }\n      ]\n    },\n    \"platformDisplayName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The name of a signing platform.\"\n        }\n      ]\n    },\n    \"signatureExpiresAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"The time when\
  \ the signature of a signing job expires.\"\n        }\n      ]\n    },\n    \"jobOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the job owner.\"\n        }\n      ]\n    },\n    \"jobInvoker\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the job invoker.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-job-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningJob
---
