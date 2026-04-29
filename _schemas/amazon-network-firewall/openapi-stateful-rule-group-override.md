---
description: The setting that allows the policy owner to change the behavior of the rule group within a policy.
layout: schema
name: StatefulRuleGroupOverride
properties_list:
- description: ''
  name: Action
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateful-rule-group-override-schema.json
slug: openapi-stateful-rule-group-override
source_filename: openapi-stateful-rule-group-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-group-override-schema.json\",\n  \"title\": \"StatefulRuleGroupOverride\",\n  \"description\": \"The setting that allows the policy owner to change the behavior of the rule group within a policy. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverrideAction\"\n        },\n        {\n          \"description\": \"The action that changes the rule group from <code>DROP</code> to <code>ALERT</code>. This only applies to managed rule groups.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateful-rule-group-override-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatefulRuleGroupOverride
---
