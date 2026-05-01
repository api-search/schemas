---
description: Contains other private IP address information of the EC2 instance.
layout: schema
name: PrivateIpAddressDetails
properties_list:
- description: ''
  name: PrivateDnsName
  type: object
- description: ''
  name: PrivateIpAddress
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-private-ip-address-details-schema.json
slug: guardduty-private-ip-address-details
source_filename: guardduty-private-ip-address-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-private-ip-address-details-schema.json\",\n  \"title\": \"PrivateIpAddressDetails\",\n  \"description\": \"Contains other private IP address information of the EC2 instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrivateDnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateDnsName\"\n          },\n          \"description\": \"The private DNS name of the EC2 instance.\"\n        }\n      ]\n    },\n    \"PrivateIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateIpAddress\"\n          },\n          \"description\": \"The private IP address\
  \ of the EC2 instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-private-ip-address-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: PrivateIpAddressDetails
---
