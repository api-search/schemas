---
description: Points to an <code>S3SignedObject</code> object that contains information about your signed code image.
layout: schema
name: SignedObject
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signed-object-schema.json
slug: amazon-signer-signed-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signed-object-schema.json\",\n  \"title\": \"SignedObject\",\n  \"description\": \"Points to an <code>S3SignedObject</code> object that contains information about your signed code image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bucketName\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/BucketName\"\n                },\n                {\n                  \"description\": \"Name of the S3 bucket.\"\n                }\n              ]\n            },\n            \"key\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/Key\"\n                },\n         \
  \       {\n                  \"description\": \"Key name that uniquely identifies a signed code image in your bucket.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The S3 bucket name and key where code signing saved your signed code image.\"\n        },\n        {\n          \"description\": \"The <code>S3SignedObject</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signed-object-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SignedObject
---
