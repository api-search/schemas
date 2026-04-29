---
description: Contains information about the account level permissions on the S3 bucket.
layout: schema
name: AccountLevelPermissions
properties_list:
- description: ''
  name: BlockPublicAccess
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-account-level-permissions-schema.json
slug: guardduty-account-level-permissions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-account-level-permissions-schema.json\",\n  \"title\": \"AccountLevelPermissions\",\n  \"description\": \"Contains information about the account level permissions on the S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlockPublicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockPublicAccess\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blockPublicAccess\"\n          },\n          \"description\": \"Describes the S3 Block Public Access settings of the bucket's parent account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-account-level-permissions-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AccountLevelPermissions
---
