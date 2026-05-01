---
description: Contains information about the bucket level permissions for the S3 bucket.
layout: schema
name: BucketLevelPermissions
properties_list:
- description: ''
  name: AccessControlList
  type: object
- description: ''
  name: BucketPolicy
  type: object
- description: ''
  name: BlockPublicAccess
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-bucket-level-permissions-schema.json
slug: guardduty-bucket-level-permissions
source_filename: guardduty-bucket-level-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-bucket-level-permissions-schema.json\",\n  \"title\": \"BucketLevelPermissions\",\n  \"description\": \"Contains information about the bucket level permissions for the S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessControlList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accessControlList\"\n          },\n          \"description\": \"Contains information on how Access Control Policies are applied to the bucket.\"\n        }\n      ]\n    },\n    \"BucketPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketPolicy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bucketPolicy\"\n    \
  \      },\n          \"description\": \"Contains information on the bucket policies for the S3 bucket.\"\n        }\n      ]\n    },\n    \"BlockPublicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockPublicAccess\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blockPublicAccess\"\n          },\n          \"description\": \"Contains information on which account level S3 Block Public Access settings are applied to the S3 bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-bucket-level-permissions-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: BucketLevelPermissions
---
