---
description: Access configuration parameters.
layout: schema
name: AccessConfiguration
properties_list:
- description: ''
  name: AccessType
  type: object
- description: ''
  name: SecretsManagerAccessTokenConfiguration
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-access-configuration-schema.json
slug: mediatailor-api-access-configuration
source_filename: mediatailor-api-access-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-access-configuration-schema.json\",\n  \"title\": \"AccessConfiguration\",\n  \"description\": \"Access configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessType\"\n        },\n        {\n          \"description\": \"<p>The type of authentication used to access content from <code>HttpConfiguration::BaseUrl</code> on your source location. Accepted value: <code>S3_SIGV4</code>.</p> <p> <code>S3_SIGV4</code> - AWS Signature Version 4 authentication for Amazon S3 hosted virtual-style access. If your source location base URL is an Amazon S3 bucket, MediaTailor can use AWS Signature Version 4 (SigV4) authentication to access the bucket where your source content is stored.\
  \ Your MediaTailor source location baseURL must follow the S3 virtual hosted-style request URL format. For example, https://bucket-name.s3.Region.amazonaws.com/key-name.</p> <p>Before you can use <code>S3_SIGV4</code>, you must meet these requirements:</p> <p>\\u2022 You must allow MediaTailor to access your S3 bucket by granting mediatailor.amazonaws.com principal access in IAM. For information about configuring access in IAM, see Access management in the IAM User Guide.</p> <p>\\u2022 The mediatailor.amazonaws.com service principal must have permissions to read all top level manifests referenced by the VodSource packaging configurations.</p> <p>\\u2022 The caller of the API must have s3:GetObject IAM permissions to read all top level manifests referenced by your MediaTailor VodSource packaging configurations.</p>\"\n        }\n      ]\n    },\n    \"SecretsManagerAccessTokenConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretsManagerAccessTokenConfiguration\"\
  \n        },\n        {\n          \"description\": \"AWS Secrets Manager access token configuration parameters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-access-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AccessConfiguration
---
