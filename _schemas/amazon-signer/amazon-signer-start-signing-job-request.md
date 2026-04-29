---
description: StartSigningJobRequest schema from AWS Signer API
layout: schema
name: StartSigningJobRequest
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: profileName
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: profileOwner
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-start-signing-job-request-schema.json
slug: amazon-signer-start-signing-job-request
source_filename: amazon-signer-start-signing-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-start-signing-job-request-schema.json\",\n  \"title\": \"StartSigningJobRequest\",\n  \"description\": \"StartSigningJobRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"s3\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/S3Source\"\n                },\n                {\n                  \"description\": \"The <code>S3Source</code> object.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"An <code>S3Source</code> object that contains information about the S3 bucket where you saved your unsigned code.\"\n        },\n        {\n   \
  \       \"description\": \"The S3 bucket that contains the object to sign or a BLOB that contains your raw code.\"\n        }\n      ]\n    },\n    \"destination\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"s3\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/S3Destination\"\n                },\n                {\n                  \"description\": \"The <code>S3Destination</code> object.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Points to an <code>S3Destination</code> object that contains information about your S3 bucket.\"\n        },\n        {\n          \"description\": \"The S3 bucket in which to save your signed object. The destination contains the name of your bucket and an optional prefix.\"\n        }\n      ]\n    },\n    \"profileName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\
  ,\n          \"pattern\": \"^[a-zA-Z0-9_]{2,}\",\n          \"minLength\": 2,\n          \"maxLength\": 64\n        },\n        {\n          \"description\": \"The name of the signing profile.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"String that identifies the signing request. All calls after the first that use this token return the same response as the first call.\"\n        }\n      ]\n    },\n    \"profileOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the signing profile owner.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"destination\",\n    \"profileName\",\n    \"clientRequestToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-start-signing-job-request-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: StartSigningJobRequest
---
