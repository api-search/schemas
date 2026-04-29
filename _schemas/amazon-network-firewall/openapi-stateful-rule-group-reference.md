---
description: Identifier for a single stateful rule group, used in a firewall policy to refer to a rule group.
layout: schema
name: StatefulRuleGroupReference
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Override
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateful-rule-group-reference-schema.json
slug: openapi-stateful-rule-group-reference
source_filename: openapi-stateful-rule-group-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-group-reference-schema.json\",\n  \"title\": \"StatefulRuleGroupReference\",\n  \"description\": \"Identifier for a single stateful rule group, used in a firewall policy to refer to a rule group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the stateful rule group.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"<p>An integer setting that indicates the order in which to run the stateful rule groups in a single <a>FirewallPolicy</a>.\
  \ This setting only applies to firewall policies that specify the <code>STRICT_ORDER</code> rule order in the stateful engine options settings.</p> <p>Network Firewall evalutes each stateful rule group against a packet starting with the group that has the lowest priority setting. You must ensure that the priority settings are unique within each policy.</p> <p>You can change the priority settings of your rule groups at any time. To make it easier to insert rule groups later, number them so there's a wide range in between, for example use 100, 200, and so on. </p>\"\n        }\n      ]\n    },\n    \"Override\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatefulRuleGroupOverride\"\n        },\n        {\n          \"description\": \"The action that allows the policy owner to override the behavior of the rule group within a policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-group-reference-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatefulRuleGroupReference
---
