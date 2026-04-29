---
description: Information about the installed EKS add-on (GuardDuty security agent).
layout: schema
name: AddonDetails
properties_list:
- description: ''
  name: AddonVersion
  type: object
- description: ''
  name: AddonStatus
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-addon-details-schema.json
slug: guardduty-addon-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-addon-details-schema.json\",\n  \"title\": \"AddonDetails\",\n  \"description\": \"Information about the installed EKS add-on (GuardDuty security agent).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddonVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"addonVersion\"\n          },\n          \"description\": \"Version of the installed EKS add-on.\"\n        }\n      ]\n    },\n    \"AddonStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"addonStatus\"\n          },\n          \"description\": \"Status of the installed EKS add-on.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-addon-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AddonDetails
---
