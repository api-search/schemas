---
description: Volume used by the Kubernetes workload.
layout: schema
name: Volume
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: HostPath
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-volume-schema.json
slug: guardduty-volume
source_filename: guardduty-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-volume-schema.json\",\n  \"title\": \"Volume\",\n  \"description\": \"Volume used by the Kubernetes workload.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Volume name.\"\n        }\n      ]\n    },\n    \"HostPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostPath\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostPath\"\n          },\n          \"description\": \"Represents a pre-existing file or directory on the host machine that the volume maps to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-volume-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Volume
---
