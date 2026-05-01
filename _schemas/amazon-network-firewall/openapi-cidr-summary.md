---
description: Summarizes the CIDR blocks used by the IP set references in a firewall. Network Firewall calculates the number of CIDRs by taking an aggregated count of all CIDRs used by the IP sets you are referencing.
layout: schema
name: CIDRSummary
properties_list:
- description: ''
  name: AvailableCIDRCount
  type: object
- description: ''
  name: UtilizedCIDRCount
  type: object
- description: ''
  name: IPSetReferences
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-cidr-summary-schema.json
slug: openapi-cidr-summary
source_filename: openapi-cidr-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-cidr-summary-schema.json\",\n  \"title\": \"CIDRSummary\",\n  \"description\": \"Summarizes the CIDR blocks used by the IP set references in a firewall. Network Firewall calculates the number of CIDRs by taking an aggregated count of all CIDRs used by the IP sets you are referencing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailableCIDRCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDRCount\"\n        },\n        {\n          \"description\": \"The number of CIDR blocks available for use by the IP set references in a firewall.\"\n        }\n      ]\n    },\n    \"UtilizedCIDRCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDRCount\"\n        },\n        {\n          \"description\": \"The number\
  \ of CIDR blocks used by the IP set references in a firewall.\"\n        }\n      ]\n    },\n    \"IPSetReferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IPSetMetadataMap\"\n        },\n        {\n          \"description\": \"The list of the IP set references used by a firewall.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-cidr-summary-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CIDRSummary
---
