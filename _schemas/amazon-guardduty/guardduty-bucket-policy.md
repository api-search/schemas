---
description: Contains information on the current bucket policies for the S3 bucket.
layout: schema
name: BucketPolicy
properties_list:
- description: ''
  name: AllowsPublicReadAccess
  type: object
- description: ''
  name: AllowsPublicWriteAccess
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-bucket-policy-schema.json
slug: guardduty-bucket-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-bucket-policy-schema.json\",\n  \"title\": \"BucketPolicy\",\n  \"description\": \"Contains information on the current bucket policies for the S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowsPublicReadAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"allowsPublicReadAccess\"\n          },\n          \"description\": \"A value that indicates whether public read access for the bucket is enabled through a bucket policy.\"\n        }\n      ]\n    },\n    \"AllowsPublicWriteAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"allowsPublicWriteAccess\"\
  \n          },\n          \"description\": \"A value that indicates whether public write access for the bucket is enabled through a bucket policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-bucket-policy-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: BucketPolicy
---
