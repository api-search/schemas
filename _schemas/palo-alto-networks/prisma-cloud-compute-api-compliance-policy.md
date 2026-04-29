---
description: CompliancePolicy schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: CompliancePolicy
properties_list:
- description: Ordered list of compliance policy rules.
  name: rules
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-compliance-policy-schema.json
slug: prisma-cloud-compute-api-compliance-policy
source_filename: prisma-cloud-compute-api-compliance-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompliancePolicy\",\n  \"description\": \"CompliancePolicy schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-compliance-policy-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of compliance policy rules.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"collections\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"effect\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ignore\",\n              \"alert\",\n            \
  \  \"block\"\n            ]\n          },\n          \"condition\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"checks\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"integer\",\n                      \"description\": \"Compliance check ID.\"\n                    },\n                    \"block\": {\n                      \"type\": \"boolean\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-compliance-policy-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CompliancePolicy
---
