---
description: Contains information about the port probe details.
layout: schema
name: PortProbeDetail
properties_list:
- description: ''
  name: LocalPortDetails
  type: object
- description: ''
  name: LocalIpDetails
  type: object
- description: ''
  name: RemoteIpDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-port-probe-detail-schema.json
slug: guardduty-port-probe-detail
source_filename: guardduty-port-probe-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-port-probe-detail-schema.json\",\n  \"title\": \"PortProbeDetail\",\n  \"description\": \"Contains information about the port probe details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LocalPortDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocalPortDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"localPortDetails\"\n          },\n          \"description\": \"The local port information of the connection.\"\n        }\n      ]\n    },\n    \"LocalIpDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocalIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"localIpDetails\"\n          },\n          \"description\": \"The local IP information of the\
  \ connection.\"\n        }\n      ]\n    },\n    \"RemoteIpDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteIpDetails\"\n          },\n          \"description\": \"The remote IP information of the connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-port-probe-detail-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: PortProbeDetail
---
