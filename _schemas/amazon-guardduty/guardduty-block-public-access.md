---
description: Contains information on how the bucker owner's S3 Block Public Access settings are being applied to the S3 bucket. See <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html">S3 Block Public Access</a> for more information.
layout: schema
name: BlockPublicAccess
properties_list:
- description: ''
  name: IgnorePublicAcls
  type: object
- description: ''
  name: RestrictPublicBuckets
  type: object
- description: ''
  name: BlockPublicAcls
  type: object
- description: ''
  name: BlockPublicPolicy
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-block-public-access-schema.json
slug: guardduty-block-public-access
source_filename: guardduty-block-public-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-block-public-access-schema.json\",\n  \"title\": \"BlockPublicAccess\",\n  \"description\": \"Contains information on how the bucker owner's S3 Block Public Access settings are being applied to the S3 bucket. See <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/access-control-block-public-access.html\\\">S3 Block Public Access</a> for more information. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IgnorePublicAcls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ignorePublicAcls\"\n          },\n          \"description\": \"Indicates if S3 Block Public Access is set to <code>IgnorePublicAcls</code>.\"\n        }\n      ]\n    },\n    \"RestrictPublicBuckets\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"restrictPublicBuckets\"\n          },\n          \"description\": \"Indicates if S3 Block Public Access is set to <code>RestrictPublicBuckets</code>.\"\n        }\n      ]\n    },\n    \"BlockPublicAcls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blockPublicAcls\"\n          },\n          \"description\": \"Indicates if S3 Block Public Access is set to <code>BlockPublicAcls</code>.\"\n        }\n      ]\n    },\n    \"BlockPublicPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blockPublicPolicy\"\n          },\n          \"description\": \"Indicates if S3 Block Public Access is set to <code>BlockPublicPolicy</code>.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-block-public-access-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: BlockPublicAccess
---
