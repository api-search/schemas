---
description: The S3 bucket name and key where code signing saved your signed code image.
layout: schema
name: S3SignedObject
properties_list:
- description: ''
  name: bucketName
  type: object
- description: ''
  name: key
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-s3-signed-object-schema.json
slug: amazon-signer-s3-signed-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-s3-signed-object-schema.json\",\n  \"title\": \"S3SignedObject\",\n  \"description\": \"The S3 bucket name and key where code signing saved your signed code image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Key name that uniquely identifies a signed code image in your bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-s3-signed-object-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: S3SignedObject
---
