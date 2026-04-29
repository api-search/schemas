---
description: Contains information about the security groups associated with the EC2 instance.
layout: schema
name: SecurityGroup
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: GroupName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-security-group-schema.json
slug: guardduty-security-group
source_filename: guardduty-security-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-security-group-schema.json\",\n  \"title\": \"SecurityGroup\",\n  \"description\": \"Contains information about the security groups associated with the EC2 instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groupId\"\n          },\n          \"description\": \"The security group ID of the EC2 instance.\"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groupName\"\n          },\n          \"description\": \"The security group name of the EC2 instance.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-security-group-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: SecurityGroup
---
