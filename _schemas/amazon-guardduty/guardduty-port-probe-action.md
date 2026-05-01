---
description: Contains information about the PORT_PROBE action described in the finding.
layout: schema
name: PortProbeAction
properties_list:
- description: ''
  name: Blocked
  type: object
- description: ''
  name: PortProbeDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-port-probe-action-schema.json
slug: guardduty-port-probe-action
source_filename: guardduty-port-probe-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-port-probe-action-schema.json\",\n  \"title\": \"PortProbeAction\",\n  \"description\": \"Contains information about the PORT_PROBE action described in the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Blocked\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blocked\"\n          },\n          \"description\": \"Indicates whether EC2 blocked the port probe to the instance, such as with an ACL.\"\n        }\n      ]\n    },\n    \"PortProbeDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortProbeDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"portProbeDetails\"\n          },\n          \"description\"\
  : \"A list of objects related to port probe details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-port-probe-action-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: PortProbeAction
---
