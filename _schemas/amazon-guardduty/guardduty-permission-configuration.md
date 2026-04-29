---
description: Contains information about how permissions are configured for the S3 bucket.
layout: schema
name: PermissionConfiguration
properties_list:
- description: ''
  name: BucketLevelPermissions
  type: object
- description: ''
  name: AccountLevelPermissions
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-permission-configuration-schema.json
slug: guardduty-permission-configuration
source_filename: guardduty-permission-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-permission-configuration-schema.json\",\n  \"title\": \"PermissionConfiguration\",\n  \"description\": \"Contains information about how permissions are configured for the S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketLevelPermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketLevelPermissions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bucketLevelPermissions\"\n          },\n          \"description\": \"Contains information about the bucket level permissions for the S3 bucket.\"\n        }\n      ]\n    },\n    \"AccountLevelPermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountLevelPermissions\"\n        },\n        {\n          \"xml\": {\n        \
  \    \"name\": \"accountLevelPermissions\"\n          },\n          \"description\": \"Contains information about the account level permissions on the S3 bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-permission-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: PermissionConfiguration
---
