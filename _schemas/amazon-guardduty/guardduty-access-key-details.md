---
description: Contains information about the access keys.
layout: schema
name: AccessKeyDetails
properties_list:
- description: ''
  name: AccessKeyId
  type: object
- description: ''
  name: PrincipalId
  type: object
- description: ''
  name: UserName
  type: object
- description: ''
  name: UserType
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-access-key-details-schema.json
slug: guardduty-access-key-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-access-key-details-schema.json\",\n  \"title\": \"AccessKeyDetails\",\n  \"description\": \"Contains information about the access keys.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accessKeyId\"\n          },\n          \"description\": \"The access key ID of the user.\"\n        }\n      ]\n    },\n    \"PrincipalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"principalId\"\n          },\n          \"description\": \"The principal ID of the user.\"\n        }\n      ]\n    },\n    \"UserName\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userName\"\n          },\n          \"description\": \"The name of the user.\"\n        }\n      ]\n    },\n    \"UserType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userType\"\n          },\n          \"description\": \"The type of the user.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-access-key-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AccessKeyDetails
---
