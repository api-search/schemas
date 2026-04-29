---
description: Represents a pre-existing file or directory on the host machine that the volume maps to.
layout: schema
name: HostPath
properties_list:
- description: ''
  name: Path
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-host-path-schema.json
slug: guardduty-host-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-host-path-schema.json\",\n  \"title\": \"HostPath\",\n  \"description\": \"Represents a pre-existing file or directory on the host machine that the volume maps to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"path\"\n          },\n          \"description\": \"Path of the file or directory on the host that the volume maps to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-host-path-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: HostPath
---
