---
description: <p>Minimal high-level information for a firewall rule group. The action <a>ListFirewallRuleGroups</a> returns an array of these objects. </p> <p>To retrieve full information for a firewall rule group, call <a>GetFirewallRuleGroup</a> and <a>ListFirewallRules</a>.</p>
layout: schema
name: FirewallRuleGroupMetadata
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: ShareStatus
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-firewall-rule-group-metadata-schema.json
slug: amazon-route53-resolver-openapi-firewall-rule-group-metadata
source_filename: amazon-route53-resolver-openapi-firewall-rule-group-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-rule-group-metadata-schema.json\",\n  \"title\": \"FirewallRuleGroupMetadata\",\n  \"description\": \"<p>Minimal high-level information for a firewall rule group. The action <a>ListFirewallRuleGroups</a> returns an array of these objects. </p> <p>To retrieve full information for a firewall rule group, call <a>GetFirewallRuleGroup</a> and <a>ListFirewallRules</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the rule group. \"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"\
  description\": \"The ARN (Amazon Resource Name) of the rule group.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the rule group.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account that created the rule group. When a rule group is shared with your account, this is the account that has shared the rule group with you. \"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string defined by you to identify the request. This allows you to retry failed requests without the risk of running the operation\
  \ twice. This can be any unique string, for example, a timestamp. \"\n        }\n      ]\n    },\n    \"ShareStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareStatus\"\n        },\n        {\n          \"description\": \"Whether the rule group is shared with other Amazon Web Services accounts, or was shared with the current account by another Amazon Web Services account. Sharing is configured through Resource Access Manager (RAM).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-rule-group-metadata-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: FirewallRuleGroupMetadata
---
