---
description: DescribeRuleGroupMetadataResponse schema from Amazon Network Firewall
layout: schema
name: DescribeRuleGroupMetadataResponse
properties_list:
- description: ''
  name: RuleGroupArn
  type: object
- description: ''
  name: RuleGroupName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Capacity
  type: object
- description: ''
  name: StatefulRuleOptions
  type: object
- description: ''
  name: LastModifiedTime
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-describe-rule-group-metadata-response-schema.json
slug: openapi-describe-rule-group-metadata-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-rule-group-metadata-response-schema.json\",\n  \"title\": \"DescribeRuleGroupMetadataResponse\",\n  \"description\": \"DescribeRuleGroupMetadataResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The descriptive name of the rule group. You can't change the name of a rule group after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"RuleGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"<p>The\
  \ descriptive name of the rule group. You can't change the name of a rule group after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Returns the metadata objects for the specified rule group. \"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the rule group is stateless or stateful. If the rule group is stateless, it contains stateless rules. If it is stateful, it contains stateful rules. </p> <note> <p>This setting is required for requests that do not include the <code>RuleGroupARN</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"Capacity\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/RuleCapacity\"\n        },\n        {\n          \"description\": \"<p>The maximum operating resources that this rule group can use. Rule group capacity is fixed at creation. When you update a rule group, you are limited to this capacity. When you reference a rule group from a firewall policy, Network Firewall reserves this capacity for the rule group. </p> <p>You can retrieve the capacity that would be required for a rule group before you create the rule group by calling <a>CreateRuleGroup</a> with <code>DryRun</code> set to <code>TRUE</code>. </p>\"\n        }\n      ]\n    },\n    \"StatefulRuleOptions\": {\n      \"$ref\": \"#/components/schemas/StatefulRuleOptions\"\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdateTime\"\n        },\n        {\n          \"description\": \"The last time that the rule group was changed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"RuleGroupArn\",\n    \"RuleGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-rule-group-metadata-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DescribeRuleGroupMetadataResponse
---
