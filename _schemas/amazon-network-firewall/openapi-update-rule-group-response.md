---
description: UpdateRuleGroupResponse schema from Amazon Network Firewall
layout: schema
name: UpdateRuleGroupResponse
properties_list:
- description: ''
  name: UpdateToken
  type: object
- description: ''
  name: RuleGroupResponse
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-update-rule-group-response-schema.json
slug: openapi-update-rule-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-rule-group-response-schema.json\",\n  \"title\": \"UpdateRuleGroupResponse\",\n  \"description\": \"UpdateRuleGroupResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>A token used for optimistic locking. Network Firewall returns a token to your requests that access the rule group. The token marks the state of the rule group resource at the time of the request. </p> <p>To make changes to the rule group, you provide the token in your request. Network Firewall uses the token to ensure that the rule group hasn't changed since you last retrieved it. If it has changed, the operation\
  \ fails with an <code>InvalidTokenException</code>. If this happens, retrieve the rule group again to get a current copy of it with a current token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    },\n    \"RuleGroupResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupResponse\"\n        },\n        {\n          \"description\": \"The high-level properties of a rule group. This, along with the <a>RuleGroup</a>, define the rule group. You can retrieve all objects for a rule group by calling <a>DescribeRuleGroup</a>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UpdateToken\",\n    \"RuleGroupResponse\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-rule-group-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UpdateRuleGroupResponse
---
