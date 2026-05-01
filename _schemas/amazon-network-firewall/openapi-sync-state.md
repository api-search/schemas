---
description: '<p>The status of the firewall endpoint and firewall policy configuration for a single VPC subnet. </p> <p>For each VPC subnet that you associate with a firewall, Network Firewall does the following: </p> <ul> <li> <p>Instantiates a firewall endpoint in the subnet, ready to take traffic.</p> </li> <li> <p>Configures the endpoint with the current firewall policy settings, to provide the filtering behavior for the endpoint.</p> </li> </ul> <p>When you update a firewall, for example to add a subnet association or change a rule group in the firewall policy, the affected sync states reflect out-of-sync or not ready status until the changes are complete. </p>'
layout: schema
name: SyncState
properties_list:
- description: ''
  name: Attachment
  type: object
- description: ''
  name: Config
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-sync-state-schema.json
slug: openapi-sync-state
source_filename: openapi-sync-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-sync-state-schema.json\",\n  \"title\": \"SyncState\",\n  \"description\": \"<p>The status of the firewall endpoint and firewall policy configuration for a single VPC subnet. </p> <p>For each VPC subnet that you associate with a firewall, Network Firewall does the following: </p> <ul> <li> <p>Instantiates a firewall endpoint in the subnet, ready to take traffic.</p> </li> <li> <p>Configures the endpoint with the current firewall policy settings, to provide the filtering behavior for the endpoint.</p> </li> </ul> <p>When you update a firewall, for example to add a subnet association or change a rule group in the firewall policy, the affected sync states reflect out-of-sync or not ready status until the changes are complete. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attachment\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attachment\"\n        },\n        {\n          \"description\": \"The attachment status of the firewall's association with a single VPC subnet. For each configured subnet, Network Firewall creates the attachment by instantiating the firewall endpoint in the subnet so that it's ready to take traffic. This is part of the <a>FirewallStatus</a>.\"\n        }\n      ]\n    },\n    \"Config\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncStateConfig\"\n        },\n        {\n          \"description\": \"The configuration status of the firewall endpoint in a single VPC subnet. Network Firewall provides each endpoint with the rules that are configured in the firewall policy. Each time you add a subnet or modify the associated firewall policy, Network Firewall synchronizes the rules in the endpoint, so it can properly filter network traffic. This is part of the <a>FirewallStatus</a>.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-sync-state-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: SyncState
---
