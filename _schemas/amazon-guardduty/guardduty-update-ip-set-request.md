---
description: UpdateIPSetRequest schema from Amazon GuardDuty API
layout: schema
name: UpdateIPSetRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: Activate
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-ip-set-request-schema.json
slug: guardduty-update-ip-set-request
source_filename: guardduty-update-ip-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-ip-set-request-schema.json\",\n  \"title\": \"UpdateIPSetRequest\",\n  \"description\": \"UpdateIPSetRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The unique ID that specifies the IPSet that you want to update.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Location\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"location\"\n          },\n          \"description\": \"The updated URI of the file that contains the IPSet. \"\n\
  \        }\n      ]\n    },\n    \"Activate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activate\"\n          },\n          \"description\": \"The updated Boolean value that specifies whether the IPSet is active or not.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-ip-set-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdateIPSetRequest
---
