---
description: CreateRuleGroupRequest schema from Amazon Network Firewall
layout: schema
name: CreateRuleGroupRequest
properties_list:
- description: ''
  name: RuleGroupName
  type: object
- description: ''
  name: RuleGroup
  type: object
- description: ''
  name: Rules
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Capacity
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
- description: ''
  name: SourceMetadata
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-create-rule-group-request-schema.json
slug: openapi-create-rule-group-request
source_filename: openapi-create-rule-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-rule-group-request-schema.json\",\n  \"title\": \"CreateRuleGroupRequest\",\n  \"description\": \"CreateRuleGroupRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the rule group. You can't change the name of a rule group after you create it.\"\n        }\n      ]\n    },\n    \"RuleGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroup\"\n        },\n        {\n          \"description\": \"<p>An object that defines the rule group rules. </p> <note> <p>You must provide either this rule group setting or a <code>Rules</code>\
  \ setting, but not both. </p> </note>\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesString\"\n        },\n        {\n          \"description\": \"<p>A string containing stateful rule group rules specifications in Suricata flat format, with one rule per line. Use this to import your existing Suricata compatible rule groups. </p> <note> <p>You must provide either this rules setting or a populated <code>RuleGroup</code> setting, but not both. </p> </note> <p>You can provide your rule group specification in Suricata flat format through this setting when you create or update your rule group. The call response returns a <a>RuleGroup</a> object that Network Firewall has populated from your string. </p>\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupType\"\n        },\n        {\n          \"description\": \"Indicates whether the\
  \ rule group is stateless or stateful. If the rule group is stateless, it contains stateless rules. If it is stateful, it contains stateful rules. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the rule group. \"\n        }\n      ]\n    },\n    \"Capacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleCapacity\"\n        },\n        {\n          \"description\": \"<p>The maximum operating resources that this rule group can use. Rule group capacity is fixed at creation. When you update a rule group, you are limited to this capacity. When you reference a rule group from a firewall policy, Network Firewall reserves this capacity for the rule group. </p> <p>You can retrieve the capacity that would be required for a rule group before you create the rule group by calling <a>CreateRuleGroup</a>\
  \ with <code>DryRun</code> set to <code>TRUE</code>. </p> <note> <p>You can't change or exceed this capacity when you update the rule group, so leave room for your rule group to grow. </p> </note> <p> <b>Capacity for a stateless rule group</b> </p> <p>For a stateless rule group, the capacity required is the sum of the capacity requirements of the individual rules that you expect to have in the rule group. </p> <p>To calculate the capacity requirement of a single rule, multiply the capacity requirement values of each of the rule's match settings:</p> <ul> <li> <p>A match setting with no criteria specified has a value of 1. </p> </li> <li> <p>A match setting with <code>Any</code> specified has a value of 1. </p> </li> <li> <p>All other match settings have a value equal to the number of elements provided in the setting. For example, a protocol setting [\\\"UDP\\\"] and a source setting [\\\"10.0.0.0/24\\\"] each have a value of 1. A protocol setting [\\\"UDP\\\",\\\"TCP\\\"] has a value of\
  \ 2. A source setting [\\\"10.0.0.0/24\\\",\\\"10.0.0.1/24\\\",\\\"10.0.0.2/24\\\"] has a value of 3. </p> </li> </ul> <p>A rule with no criteria specified in any of its match settings has a capacity requirement of 1. A rule with protocol setting [\\\"UDP\\\",\\\"TCP\\\"], source setting [\\\"10.0.0.0/24\\\",\\\"10.0.0.1/24\\\",\\\"10.0.0.2/24\\\"], and a single specification or no specification for each of the other match settings has a capacity requirement of 6. </p> <p> <b>Capacity for a stateful rule group</b> </p> <p>For a stateful rule group, the minimum capacity required is the number of individual rules that you expect to have in the rule group. </p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether you want Network Firewall to just check the validity of the request, rather than run the request. </p> <p>If set to <code>TRUE</code>, Network Firewall checks whether the request can run successfully, but doesn't actually make the requested changes. The call returns the value that the request would return if you ran it with dry run set to <code>FALSE</code>, but doesn't make additions or changes to your resources. This option allows you to make sure that you have the required permissions to run the request and that your request parameters are valid. </p> <p>If set to <code>FALSE</code>, Network Firewall makes the requested changes to your resources. </p>\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex\
  \ type that contains settings for encryption of your rule group resources.\"\n        }\n      ]\n    },\n    \"SourceMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceMetadata\"\n        },\n        {\n          \"description\": \"A complex type that contains metadata about the rule group that your own rule group is copied from. You can use the metadata to keep track of updates made to the originating rule group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleGroupName\",\n    \"Type\",\n    \"Capacity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-create-rule-group-request-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CreateRuleGroupRequest
---
