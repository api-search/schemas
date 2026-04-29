---
description: Points to an <code>S3Destination</code> object that contains information about your S3 bucket.
layout: schema
name: Destination
properties_list:
- description: ''
  name: s3
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-destination-schema.json
slug: amazon-signer-destination
source_filename: amazon-signer-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-destination-schema.json\",\n  \"title\": \"Destination\",\n  \"description\": \"Points to an <code>S3Destination</code> object that contains information about your S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bucketName\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/BucketName\"\n                },\n                {\n                  \"description\": \"Name of the S3 bucket.\"\n                }\n              ]\n            },\n            \"prefix\": {\n              \"allOf\": [\n                {\n                  \"$ref\": \"#/components/schemas/Prefix\"\n                },\n               \
  \ {\n                  \"description\": \"An Amazon S3 prefix that you can use to limit responses to those that begin with the specified prefix.\"\n                }\n              ]\n            }\n          },\n          \"description\": \"The name and prefix of the S3 bucket where code signing saves your signed objects.\"\n        },\n        {\n          \"description\": \"The <code>S3Destination</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-destination-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: Destination
---
