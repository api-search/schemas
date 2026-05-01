---
description: CreateFirewallRequest schema from Amazon Network Firewall
layout: schema
name: CreateFirewallRequest
properties_list:
- description: ''
  name: FirewallName
  type: object
- description: ''
  name: FirewallPolicyArn
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetMappings
  type: object
- description: ''
  name: DeleteProtection
  type: object
- description: ''
  name: SubnetChangeProtection
  type: object
- description: ''
  name: FirewallPolicyChangeProtection
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-create-firewall-request-schema.json
slug: openapi-create-firewall-request
source_filename: openapi-create-firewall-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-firewall-request-schema.json\",\n  \"title\": \"CreateFirewallRequest\",\n  \"description\": \"CreateFirewallRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall. You can't change the name of a firewall after you create it.\"\n        }\n      ]\n    },\n    \"FirewallPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the <a>FirewallPolicy</a> that you want to use for the firewall.\"\n        }\n     \
  \ ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"<p>The unique identifier of the VPC where Network Firewall should create the firewall. </p> <p>You can't change this setting after you create the firewall. </p>\"\n        }\n      ]\n    },\n    \"SubnetMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetMappings\"\n        },\n        {\n          \"description\": \"The public subnets to use for your Network Firewall firewalls. Each subnet must belong to a different Availability Zone in the VPC. Network Firewall creates a firewall endpoint in each subnet. \"\n        }\n      ]\n    },\n    \"DeleteProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A flag indicating whether it is possible to delete the firewall. A setting of <code>TRUE</code>\
  \ indicates that the firewall is protected against deletion. Use this setting to protect against accidentally deleting a firewall that is in use. When you create a firewall, the operation initializes this flag to <code>TRUE</code>.\"\n        }\n      ]\n    },\n    \"SubnetChangeProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A setting indicating whether the firewall is protected against changes to the subnet associations. Use this setting to protect against accidentally modifying the subnet associations for a firewall that is in use. When you create a firewall, the operation initializes this setting to <code>TRUE</code>.\"\n        }\n      ]\n    },\n    \"FirewallPolicyChangeProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A setting indicating whether the firewall is protected\
  \ against a change to the firewall policy association. Use this setting to protect against accidentally modifying the firewall policy for a firewall that is in use. When you create a firewall, the operation initializes this setting to <code>TRUE</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the firewall.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains settings for encryption of your firewall\
  \ resources.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallName\",\n    \"FirewallPolicyArn\",\n    \"VpcId\",\n    \"SubnetMappings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-firewall-request-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CreateFirewallRequest
---
