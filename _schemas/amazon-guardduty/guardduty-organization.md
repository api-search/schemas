---
description: Contains information about the ISP organization of the remote IP address.
layout: schema
name: Organization
properties_list:
- description: ''
  name: Asn
  type: object
- description: ''
  name: AsnOrg
  type: object
- description: ''
  name: Isp
  type: object
- description: ''
  name: Org
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-schema.json
slug: guardduty-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"Contains information about the ISP organization of the remote IP address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Asn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"asn\"\n          },\n          \"description\": \"The Autonomous System Number (ASN) of the internet provider of the remote IP address.\"\n        }\n      ]\n    },\n    \"AsnOrg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"asnOrg\"\n          },\n          \"description\": \"The organization that registered this\
  \ ASN.\"\n        }\n      ]\n    },\n    \"Isp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"isp\"\n          },\n          \"description\": \"The ISP information for the internet provider.\"\n        }\n      ]\n    },\n    \"Org\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"org\"\n          },\n          \"description\": \"The name of the internet provider.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Organization
---
