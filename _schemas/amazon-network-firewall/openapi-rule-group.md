---
description: <p>The object that defines the rules in a rule group. This, along with <a>RuleGroupResponse</a>, define the rule group. You can retrieve all objects for a rule group by calling <a>DescribeRuleGroup</a>. </p> <p>Network Firewall uses a rule group to inspect and control network traffic. You define stateless rule groups to inspect individual packets and you define stateful rule groups to inspect packets in the context of their traffic flow. </p> <p>To use a rule group, you include it by reference in an Network Firewall firewall policy, then you use the policy in a firewall. You can reference a rule group from more than one firewall policy, and you can use a firewall policy in more than one firewall. </p>
layout: schema
name: RuleGroup
properties_list:
- description: ''
  name: RuleVariables
  type: object
- description: ''
  name: ReferenceSets
  type: object
- description: ''
  name: RulesSource
  type: object
- description: ''
  name: StatefulRuleOptions
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-rule-group-schema.json
slug: openapi-rule-group
source_filename: openapi-rule-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-group-schema.json\",\n  \"title\": \"RuleGroup\",\n  \"description\": \"<p>The object that defines the rules in a rule group. This, along with <a>RuleGroupResponse</a>, define the rule group. You can retrieve all objects for a rule group by calling <a>DescribeRuleGroup</a>. </p> <p>Network Firewall uses a rule group to inspect and control network traffic. You define stateless rule groups to inspect individual packets and you define stateful rule groups to inspect packets in the context of their traffic flow. </p> <p>To use a rule group, you include it by reference in an Network Firewall firewall policy, then you use the policy in a firewall. You can reference a rule group from more than one firewall policy, and you can use a firewall policy in more than one firewall. </p>\",\n  \"\
  type\": \"object\",\n  \"properties\": {\n    \"RuleVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleVariables\"\n        },\n        {\n          \"description\": \"Settings that are available for use in the rules in the rule group. You can only use these for stateful rule groups. \"\n        }\n      ]\n    },\n    \"ReferenceSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceSets\"\n        },\n        {\n          \"description\": \"The list of a rule group's reference sets.\"\n        }\n      ]\n    },\n    \"RulesSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesSource\"\n        },\n        {\n          \"description\": \"The stateful rules or stateless rules for the rule group. \"\n        }\n      ]\n    },\n    \"StatefulRuleOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatefulRuleOptions\"\n        },\n\
  \        {\n          \"description\": \"Additional options governing how Network Firewall handles stateful rules. The policies where you use your stateful rule group must have stateful rule options settings that are compatible with these settings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RulesSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-group-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: RuleGroup
---
