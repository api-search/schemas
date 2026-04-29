---
description: The capacity usage summary of the resources used by the <a>ReferenceSets</a> in a firewall.
layout: schema
name: CapacityUsageSummary
properties_list:
- description: ''
  name: CIDRs
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-capacity-usage-summary-schema.json
slug: openapi-capacity-usage-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-capacity-usage-summary-schema.json\",\n  \"title\": \"CapacityUsageSummary\",\n  \"description\": \"The capacity usage summary of the resources used by the <a>ReferenceSets</a> in a firewall.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CIDRs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDRSummary\"\n        },\n        {\n          \"description\": \"Describes the capacity usage of the CIDR blocks used by the IP set references in a firewall.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-capacity-usage-summary-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CapacityUsageSummary
---
