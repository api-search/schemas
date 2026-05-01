---
description: Container volume mount.
layout: schema
name: VolumeMount
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: MountPath
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-volume-mount-schema.json
slug: guardduty-volume-mount
source_filename: guardduty-volume-mount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-volume-mount-schema.json\",\n  \"title\": \"VolumeMount\",\n  \"description\": \"Container volume mount.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Volume mount name.\"\n        }\n      ]\n    },\n    \"MountPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mountPath\"\n          },\n          \"description\": \"Volume mount path.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-volume-mount-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: VolumeMount
---
