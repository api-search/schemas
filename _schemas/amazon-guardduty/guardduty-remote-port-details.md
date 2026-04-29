---
description: Contains information about the remote port.
layout: schema
name: RemotePortDetails
properties_list:
- description: ''
  name: Port
  type: object
- description: ''
  name: PortName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-remote-port-details-schema.json
slug: guardduty-remote-port-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-remote-port-details-schema.json\",\n  \"title\": \"RemotePortDetails\",\n  \"description\": \"Contains information about the remote port.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The port number of the remote connection.\"\n        }\n      ]\n    },\n    \"PortName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"portName\"\n          },\n          \"description\": \"The port name of the remote connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-remote-port-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RemotePortDetails
---
