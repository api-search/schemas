---
description: CreateFirewallPolicyRequest schema from Amazon Network Firewall
layout: schema
name: CreateFirewallPolicyRequest
properties_list:
- description: ''
  name: FirewallPolicyName
  type: object
- description: ''
  name: FirewallPolicy
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: DryRun
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-create-firewall-policy-request-schema.json
slug: openapi-create-firewall-policy-request
source_filename: openapi-create-firewall-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-firewall-policy-request-schema.json\",\n  \"title\": \"CreateFirewallPolicyRequest\",\n  \"description\": \"CreateFirewallPolicyRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallPolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall policy. You can't change the name of a firewall policy after you create it.\"\n        }\n      ]\n    },\n    \"FirewallPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallPolicy\"\n        },\n        {\n          \"description\": \"The rule groups and policy actions to use in the firewall policy.\"\n        }\n\
  \      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the firewall policy.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether you want Network Firewall to just check the validity of the request, rather than run the request. </p> <p>If set to <code>TRUE</code>, Network Firewall checks whether the request can run successfully, but doesn't actually make the requested changes. The call returns the value that the request would return if you ran it with dry run\
  \ set to <code>FALSE</code>, but doesn't make additions or changes to your resources. This option allows you to make sure that you have the required permissions to run the request and that your request parameters are valid. </p> <p>If set to <code>FALSE</code>, Network Firewall makes the requested changes to your resources. </p>\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains settings for encryption of your firewall policy resources.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallPolicyName\",\n    \"FirewallPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-firewall-policy-request-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CreateFirewallPolicyRequest
---
