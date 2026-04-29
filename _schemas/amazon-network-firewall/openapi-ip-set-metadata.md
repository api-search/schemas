---
description: General information about the IP set.
layout: schema
name: IPSetMetadata
properties_list:
- description: ''
  name: ResolvedCIDRCount
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-ip-set-metadata-schema.json
slug: openapi-ip-set-metadata
source_filename: openapi-ip-set-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-ip-set-metadata-schema.json\",\n  \"title\": \"IPSetMetadata\",\n  \"description\": \"General information about the IP set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResolvedCIDRCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDRCount\"\n        },\n        {\n          \"description\": \"Describes the total number of CIDR blocks currently in use by the IP set references in a firewall. To determine how many CIDR blocks are available for you to use in a firewall, you can call <code>AvailableCIDRCount</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-ip-set-metadata-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: IPSetMetadata
---
