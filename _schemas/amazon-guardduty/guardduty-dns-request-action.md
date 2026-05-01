---
description: Contains information about the DNS_REQUEST action described in this finding.
layout: schema
name: DnsRequestAction
properties_list:
- description: ''
  name: Domain
  type: object
- description: ''
  name: Protocol
  type: object
- description: ''
  name: Blocked
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-dns-request-action-schema.json
slug: guardduty-dns-request-action
source_filename: guardduty-dns-request-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-dns-request-action-schema.json\",\n  \"title\": \"DnsRequestAction\",\n  \"description\": \"Contains information about the DNS_REQUEST action described in this finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"domain\"\n          },\n          \"description\": \"The domain information for the API request.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The network connection protocol observed in the activity\
  \ that prompted GuardDuty to generate the finding.\"\n        }\n      ]\n    },\n    \"Blocked\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blocked\"\n          },\n          \"description\": \"Indicates whether the targeted port is blocked.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-dns-request-action-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DnsRequestAction
---
