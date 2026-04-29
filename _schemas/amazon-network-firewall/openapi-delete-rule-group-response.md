---
description: DeleteRuleGroupResponse schema from Amazon Network Firewall
layout: schema
name: DeleteRuleGroupResponse
properties_list:
- description: ''
  name: RuleGroupResponse
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-delete-rule-group-response-schema.json
slug: openapi-delete-rule-group-response
source_filename: openapi-delete-rule-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-rule-group-response-schema.json\",\n  \"title\": \"DeleteRuleGroupResponse\",\n  \"description\": \"DeleteRuleGroupResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleGroupResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupResponse\"\n        },\n        {\n          \"description\": \"The high-level properties of a rule group. This, along with the <a>RuleGroup</a>, define the rule group. You can retrieve all objects for a rule group by calling <a>DescribeRuleGroup</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleGroupResponse\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-delete-rule-group-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DeleteRuleGroupResponse
---
