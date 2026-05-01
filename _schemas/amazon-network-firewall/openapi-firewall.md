---
description: <p>The firewall defines the configuration settings for an Network Firewall firewall. These settings include the firewall policy, the subnets in your VPC to use for the firewall endpoints, and any tags that are attached to the firewall Amazon Web Services resource. </p> <p>The status of the firewall, for example whether it's ready to filter network traffic, is provided in the corresponding <a>FirewallStatus</a>. You can retrieve both objects by calling <a>DescribeFirewall</a>.</p>
layout: schema
name: Firewall
properties_list:
- description: ''
  name: FirewallName
  type: object
- description: ''
  name: FirewallArn
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
  name: FirewallId
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-firewall-schema.json
slug: openapi-firewall
source_filename: openapi-firewall-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-schema.json\",\n  \"title\": \"Firewall\",\n  \"description\": \"<p>The firewall defines the configuration settings for an Network Firewall firewall. These settings include the firewall policy, the subnets in your VPC to use for the firewall endpoints, and any tags that are attached to the firewall Amazon Web Services resource. </p> <p>The status of the firewall, for example whether it's ready to filter network traffic, is provided in the corresponding <a>FirewallStatus</a>. You can retrieve both objects by calling <a>DescribeFirewall</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name\
  \ of the firewall. You can't change the name of a firewall after you create it.\"\n        }\n      ]\n    },\n    \"FirewallArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the firewall.\"\n        }\n      ]\n    },\n    \"FirewallPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the firewall policy.</p> <p>The relationship of firewall to firewall policy is many to one. Each firewall requires one firewall policy association, and you can use the same firewall policy for multiple firewalls. </p>\"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The unique identifier of the VPC where\
  \ the firewall is in use. \"\n        }\n      ]\n    },\n    \"SubnetMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetMappings\"\n        },\n        {\n          \"description\": \"The public subnets that Network Firewall is using for the firewall. Each subnet must belong to a different Availability Zone. \"\n        }\n      ]\n    },\n    \"DeleteProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A flag indicating whether it is possible to delete the firewall. A setting of <code>TRUE</code> indicates that the firewall is protected against deletion. Use this setting to protect against accidentally deleting a firewall that is in use. When you create a firewall, the operation initializes this flag to <code>TRUE</code>.\"\n        }\n      ]\n    },\n    \"SubnetChangeProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\
  \n        },\n        {\n          \"description\": \"A setting indicating whether the firewall is protected against changes to the subnet associations. Use this setting to protect against accidentally modifying the subnet associations for a firewall that is in use. When you create a firewall, the operation initializes this setting to <code>TRUE</code>.\"\n        }\n      ]\n    },\n    \"FirewallPolicyChangeProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A setting indicating whether the firewall is protected against a change to the firewall policy association. Use this setting to protect against accidentally modifying the firewall policy for a firewall that is in use. When you create a firewall, the operation initializes this setting to <code>TRUE</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\
  \n        },\n        {\n          \"description\": \"A description of the firewall.\"\n        }\n      ]\n    },\n    \"FirewallId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the firewall. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains the Amazon Web Services KMS encryption configuration settings for your firewall.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallPolicyArn\",\n    \"VpcId\",\n    \"SubnetMappings\",\n    \"FirewallId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: Firewall
---
