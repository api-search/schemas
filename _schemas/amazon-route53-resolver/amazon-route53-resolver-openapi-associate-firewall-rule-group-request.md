---
description: AssociateFirewallRuleGroupRequest schema from openapi
layout: schema
name: AssociateFirewallRuleGroupRequest
properties_list:
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: FirewallRuleGroupId
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: MutationProtection
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-associate-firewall-rule-group-request-schema.json
slug: amazon-route53-resolver-openapi-associate-firewall-rule-group-request
source_filename: amazon-route53-resolver-openapi-associate-firewall-rule-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-firewall-rule-group-request-schema.json\",\n  \"title\": \"AssociateFirewallRuleGroupRequest\",\n  \"description\": \"AssociateFirewallRuleGroupRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request and that allows failed requests to be retried without the risk of running the operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. \"\n        }\n      ]\n    },\n    \"FirewallRuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\
  \n        },\n        {\n          \"description\": \"The unique identifier of the firewall rule group. \"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the VPC that you want to associate with the rule group. \"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"<p>The setting that determines the processing order of the rule group among the rule groups that you associate with the specified VPC. DNS Firewall filters VPC traffic starting from the rule group with the lowest numeric priority setting. </p> <p>You must specify a unique priority for each rule group that you associate with a single VPC. To make it easier to insert rule groups later, leave space between the numbers, for example, use\
  \ 101, 200, and so on. You can change the priority setting for a rule group association after you create it.</p> <p>The allowed values for <code>Priority</code> are between 100 and 9900.</p>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"A name that lets you identify the association, to manage and use it.\"\n        }\n      ]\n    },\n    \"MutationProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MutationProtectionStatus\"\n        },\n        {\n          \"description\": \"If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections. When you create the association, the default setting is <code>DISABLED</code>. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\
  \n        },\n        {\n          \"description\": \"A list of the tag keys and values that you want to associate with the rule group association. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatorRequestId\",\n    \"FirewallRuleGroupId\",\n    \"VpcId\",\n    \"Priority\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-associate-firewall-rule-group-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: AssociateFirewallRuleGroupRequest
---
