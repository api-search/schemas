---
description: UpdateSubnetChangeProtectionResponse schema from Amazon Network Firewall
layout: schema
name: UpdateSubnetChangeProtectionResponse
properties_list:
- description: ''
  name: UpdateToken
  type: object
- description: ''
  name: FirewallArn
  type: object
- description: ''
  name: FirewallName
  type: object
- description: ''
  name: SubnetChangeProtection
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-update-subnet-change-protection-response-schema.json
slug: openapi-update-subnet-change-protection-response
source_filename: openapi-update-subnet-change-protection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-subnet-change-protection-response-schema.json\",\n  \"title\": \"UpdateSubnetChangeProtectionResponse\",\n  \"description\": \"UpdateSubnetChangeProtectionResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>An optional token that you can use for optimistic locking. Network Firewall returns a token to your requests that access the firewall. The token marks the state of the firewall resource at the time of the request. </p> <p>To make an unconditional change to the firewall, omit the token in your update request. Without the token, Network Firewall performs your updates regardless\
  \ of whether the firewall has changed since you last retrieved it.</p> <p>To make a conditional change to the firewall, provide the token in your update request. Network Firewall uses the token to ensure that the firewall hasn't changed since you last retrieved it. If it has changed, the operation fails with an <code>InvalidTokenException</code>. If this happens, retrieve the firewall again to get a current copy of it with a new token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    },\n    \"FirewallArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the firewall.\"\n        }\n      ]\n    },\n    \"FirewallName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall.\
  \ You can't change the name of a firewall after you create it.\"\n        }\n      ]\n    },\n    \"SubnetChangeProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A setting indicating whether the firewall is protected against changes to the subnet associations. Use this setting to protect against accidentally modifying the subnet associations for a firewall that is in use. When you create a firewall, the operation initializes this setting to <code>TRUE</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-subnet-change-protection-response-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UpdateSubnetChangeProtectionResponse
---
