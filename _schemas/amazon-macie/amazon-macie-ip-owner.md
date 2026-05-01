---
description: Provides information about the registered owner of an IP address.
layout: schema
name: IpOwner
properties_list:
- description: ''
  name: asn
  type: object
- description: ''
  name: asnOrg
  type: object
- description: ''
  name: isp
  type: object
- description: ''
  name: org
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-ip-owner-schema.json
slug: amazon-macie-ip-owner
source_filename: amazon-macie-ip-owner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-owner-schema.json\",\n  \"title\": \"IpOwner\",\n  \"description\": \"Provides information about the registered owner of an IP address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The autonomous system number (ASN) for the autonomous system that included the IP address.\"\n        }\n      ]\n    },\n    \"asnOrg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The organization identifier that's associated with the autonomous system number (ASN) for the autonomous system that included the IP address.\"\n        }\n      ]\n    },\n    \"isp\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the internet service provider (ISP) that owned the IP address.\"\n        }\n      ]\n    },\n    \"org\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the organization that owned the IP address.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-ip-owner-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: IpOwner
---
