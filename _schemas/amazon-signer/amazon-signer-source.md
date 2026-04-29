---
description: An <code>S3Source</code> object that contains information about the S3 bucket where you saved your unsigned code.
layout: schema
name: Source
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-source-schema.json
slug: amazon-signer-source
source_filename: amazon-signer-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-source-schema.json\",\n  \"title\": \"Source\",\n  \"description\": \"An <code>S3Source</code> object that contains information about the S3 bucket where you saved your unsigned code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"required\": [\n            \"bucketName\",\n            \"key\",\n            \"version\"\n          ],\n          \"properties\": {\n            \"bucketName\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/BucketName\"\n                },\n                {\n                  \"description\": \"Name of the S3 bucket.\"\n                }\n              ]\n            },\n            \"key\": {\n              \"allOf\"\
  : [\n                {\n                  \"$ref\": \"#/components/schemas/Key\"\n                },\n                {\n                  \"description\": \"Key name of the bucket object that contains your unsigned code.\"\n                }\n              ]\n            },\n            \"version\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/Version\"\n                },\n                {\n                  \"description\": \"Version of your source image in your version enabled S3 bucket.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"Information about the S3 bucket where you saved your unsigned code.\"\n        },\n        {\n          \"description\": \"The <code>S3Source</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-source-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: Source
---
