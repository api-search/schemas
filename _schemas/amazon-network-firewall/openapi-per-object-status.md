---
description: Provides configuration status for a single policy or rule group that is used for a firewall endpoint. Network Firewall provides each endpoint with the rules that are configured in the firewall policy. Each time you add a subnet or modify the associated firewall policy, Network Firewall synchronizes the rules in the endpoint, so it can properly filter network traffic. This is part of a <a>SyncState</a> for a firewall.
layout: schema
name: PerObjectStatus
properties_list:
- description: ''
  name: SyncStatus
  type: object
- description: ''
  name: UpdateToken
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-per-object-status-schema.json
slug: openapi-per-object-status
source_filename: openapi-per-object-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-per-object-status-schema.json\",\n  \"title\": \"PerObjectStatus\",\n  \"description\": \"Provides configuration status for a single policy or rule group that is used for a firewall endpoint. Network Firewall provides each endpoint with the rules that are configured in the firewall policy. Each time you add a subnet or modify the associated firewall policy, Network Firewall synchronizes the rules in the endpoint, so it can properly filter network traffic. This is part of a <a>SyncState</a> for a firewall.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SyncStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PerObjectSyncStatus\"\n        },\n        {\n          \"description\": \"Indicates whether this object is in sync with the version indicated\
  \ in the update token.\"\n        }\n      ]\n    },\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"The current version of the object that is either in sync or pending synchronization. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-per-object-status-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: PerObjectStatus
---
