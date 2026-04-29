---
description: Contains information about the local IP address of the connection.
layout: schema
name: LocalIpDetails
properties_list:
- description: ''
  name: IpAddressV4
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-local-ip-details-schema.json
slug: guardduty-local-ip-details
source_filename: guardduty-local-ip-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-local-ip-details-schema.json\",\n  \"title\": \"LocalIpDetails\",\n  \"description\": \"Contains information about the local IP address of the connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddressV4\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipAddressV4\"\n          },\n          \"description\": \"The IPv4 local address of the connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-local-ip-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: LocalIpDetails
---
