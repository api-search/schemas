---
description: Contains information about the port for the local connection.
layout: schema
name: LocalPortDetails
properties_list:
- description: ''
  name: Port
  type: object
- description: ''
  name: PortName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-local-port-details-schema.json
slug: guardduty-local-port-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-local-port-details-schema.json\",\n  \"title\": \"LocalPortDetails\",\n  \"description\": \"Contains information about the port for the local connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"port\"\n          },\n          \"description\": \"The port number of the local connection.\"\n        }\n      ]\n    },\n    \"PortName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"portName\"\n          },\n          \"description\": \"The port name of the local connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-local-port-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: LocalPortDetails
---
