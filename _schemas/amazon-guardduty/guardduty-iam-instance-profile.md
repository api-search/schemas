---
description: Contains information about the EC2 instance profile.
layout: schema
name: IamInstanceProfile
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Id
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-iam-instance-profile-schema.json
slug: guardduty-iam-instance-profile
source_filename: guardduty-iam-instance-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-iam-instance-profile-schema.json\",\n  \"title\": \"IamInstanceProfile\",\n  \"description\": \"Contains information about the EC2 instance profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The profile ARN of the EC2 instance.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The profile ID of the EC2 instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-iam-instance-profile-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: IamInstanceProfile
---
