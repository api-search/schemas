---
description: Represents the resources that were scanned in the scan entry.
layout: schema
name: ResourceDetails
properties_list:
- description: ''
  name: InstanceArn
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-resource-details-schema.json
slug: guardduty-resource-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-resource-details-schema.json\",\n  \"title\": \"ResourceDetails\",\n  \"description\": \"Represents the resources that were scanned in the scan entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instanceArn\"\n          },\n          \"description\": \"InstanceArn that was scanned in the scan entry.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-resource-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ResourceDetails
---
