---
description: High-level information about a firewall, returned by operations like create and describe. You can use the information provided in the metadata to retrieve and manage a firewall.
layout: schema
name: FirewallMetadata
properties_list:
- description: ''
  name: FirewallName
  type: object
- description: ''
  name: FirewallArn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-firewall-metadata-schema.json
slug: openapi-firewall-metadata
source_filename: openapi-firewall-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-metadata-schema.json\",\n  \"title\": \"FirewallMetadata\",\n  \"description\": \"High-level information about a firewall, returned by operations like create and describe. You can use the information provided in the metadata to retrieve and manage a firewall.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall. You can't change the name of a firewall after you create it.\"\n        }\n      ]\n    },\n    \"FirewallArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource\
  \ Name (ARN) of the firewall.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-metadata-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: FirewallMetadata
---
