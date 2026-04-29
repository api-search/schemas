---
description: The high-level properties of a firewall policy. This, along with the <a>FirewallPolicy</a>, define the policy. You can retrieve all objects for a firewall policy by calling <a>DescribeFirewallPolicy</a>.
layout: schema
name: FirewallPolicyResponse
properties_list:
- description: ''
  name: FirewallPolicyName
  type: object
- description: ''
  name: FirewallPolicyArn
  type: object
- description: ''
  name: FirewallPolicyId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: FirewallPolicyStatus
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ConsumedStatelessRuleCapacity
  type: object
- description: ''
  name: ConsumedStatefulRuleCapacity
  type: object
- description: ''
  name: NumberOfAssociations
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: LastModifiedTime
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-firewall-policy-response-schema.json
slug: openapi-firewall-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-policy-response-schema.json\",\n  \"title\": \"FirewallPolicyResponse\",\n  \"description\": \"The high-level properties of a firewall policy. This, along with the <a>FirewallPolicy</a>, define the policy. You can retrieve all objects for a firewall policy by calling <a>DescribeFirewallPolicy</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallPolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the firewall policy. You can't change the name of a firewall policy after you create it.\"\n        }\n      ]\n    },\n    \"FirewallPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n \
  \       },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the firewall policy.</p> <note> <p>If this response is for a create request that had <code>DryRun</code> set to <code>TRUE</code>, then this ARN is a placeholder that isn't attached to a valid resource.</p> </note>\"\n        }\n      ]\n    },\n    \"FirewallPolicyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the firewall policy. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the firewall policy.\"\n        }\n      ]\n    },\n    \"FirewallPolicyStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStatus\"\n        },\n        {\n          \"description\": \"The current\
  \ status of the firewall policy. You can retrieve this for a firewall policy by calling <a>DescribeFirewallPolicy</a> and providing the firewall policy's name or ARN.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"ConsumedStatelessRuleCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleCapacity\"\n        },\n        {\n          \"description\": \"The number of capacity units currently consumed by the policy's stateless rules.\"\n        }\n      ]\n    },\n    \"ConsumedStatefulRuleCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleCapacity\"\n        },\n        {\n          \"description\": \"The number of capacity units currently consumed by the policy's stateful rules.\"\n  \
  \      }\n      ]\n    },\n    \"NumberOfAssociations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfAssociations\"\n        },\n        {\n          \"description\": \"The number of firewalls that are associated with this firewall policy.\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains the Amazon Web Services KMS encryption configuration settings for your firewall policy.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdateTime\"\n        },\n        {\n          \"description\": \"The last time that the firewall policy was changed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallPolicyName\",\n    \"FirewallPolicyArn\",\n    \"FirewallPolicyId\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-policy-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: FirewallPolicyResponse
---
