---
description: Additional options governing how Network Firewall handles the rule group. You can only use these for stateful rule groups.
layout: schema
name: StatefulRuleOptions
properties_list:
- description: ''
  name: RuleOrder
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateful-rule-options-schema.json
slug: openapi-stateful-rule-options
source_filename: openapi-stateful-rule-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-options-schema.json\",\n  \"title\": \"StatefulRuleOptions\",\n  \"description\": \"Additional options governing how Network Firewall handles the rule group. You can only use these for stateful rule groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleOrder\"\n        },\n        {\n          \"description\": \"Indicates how to manage the order of the rule evaluation for the rule group. <code>DEFAULT_ACTION_ORDER</code> is the default behavior. Stateful rules are provided to the rule engine as Suricata compatible strings, and Suricata evaluates them based on certain settings. For more information, see <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/suricata-rule-evaluation-order.html\\\
  \">Evaluation order for stateful rules</a> in the <i>Network Firewall Developer Guide</i>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-options-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatefulRuleOptions
---
