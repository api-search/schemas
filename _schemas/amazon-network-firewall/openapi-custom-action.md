---
description: '<p>An optional, non-standard action to use for stateless packet handling. You can define this in addition to the standard action that you must specify. </p> <p>You define and name the custom actions that you want to be able to use, and then you reference them by name in your actions settings. </p> <p>You can use custom actions in the following places: </p> <ul> <li> <p>In a rule group''s <a>StatelessRulesAndCustomActions</a> specification. The custom actions are available for use by name inside the <code>StatelessRulesAndCustomActions</code> where you define them. You can use them for your stateless rule actions to specify what to do with a packet that matches the rule''s match attributes. </p> </li> <li> <p>In a <a>FirewallPolicy</a> specification, in <code>StatelessCustomActions</code>. The custom actions are available for use inside the policy where you define them. You can use them for the policy''s default stateless actions settings to specify what to do with packets that
  don''t match any of the policy''s stateless rules. </p> </li> </ul>'
layout: schema
name: CustomAction
properties_list:
- description: ''
  name: ActionName
  type: object
- description: ''
  name: ActionDefinition
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-custom-action-schema.json
slug: openapi-custom-action
source_filename: openapi-custom-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-custom-action-schema.json\",\n  \"title\": \"CustomAction\",\n  \"description\": \"<p>An optional, non-standard action to use for stateless packet handling. You can define this in addition to the standard action that you must specify. </p> <p>You define and name the custom actions that you want to be able to use, and then you reference them by name in your actions settings. </p> <p>You can use custom actions in the following places: </p> <ul> <li> <p>In a rule group's <a>StatelessRulesAndCustomActions</a> specification. The custom actions are available for use by name inside the <code>StatelessRulesAndCustomActions</code> where you define them. You can use them for your stateless rule actions to specify what to do with a packet that matches the rule's match attributes. </p> </li> <li> <p>In\
  \ a <a>FirewallPolicy</a> specification, in <code>StatelessCustomActions</code>. The custom actions are available for use inside the policy where you define them. You can use them for the policy's default stateless actions settings to specify what to do with packets that don't match any of the policy's stateless rules. </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n        },\n        {\n          \"description\": \"The descriptive name of the custom action. You can't change the name of a custom action after you create it.\"\n        }\n      ]\n    },\n    \"ActionDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionDefinition\"\n        },\n        {\n          \"description\": \"The custom action associated with the action name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ActionName\",\n    \"\
  ActionDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-custom-action-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: CustomAction
---
