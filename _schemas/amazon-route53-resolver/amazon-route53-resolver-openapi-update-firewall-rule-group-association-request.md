---
description: UpdateFirewallRuleGroupAssociationRequest schema from openapi
layout: schema
name: UpdateFirewallRuleGroupAssociationRequest
properties_list:
- description: ''
  name: FirewallRuleGroupAssociationId
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: MutationProtection
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-update-firewall-rule-group-association-request-schema.json
slug: amazon-route53-resolver-openapi-update-firewall-rule-group-association-request
source_filename: amazon-route53-resolver-openapi-update-firewall-rule-group-association-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-firewall-rule-group-association-request-schema.json\",\n  \"title\": \"UpdateFirewallRuleGroupAssociationRequest\",\n  \"description\": \"UpdateFirewallRuleGroupAssociationRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupAssociationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the <a>FirewallRuleGroupAssociation</a>. \"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"<p>The setting that determines the processing order of the rule group among the rule\
  \ groups that you associate with the specified VPC. DNS Firewall filters VPC traffic starting from the rule group with the lowest numeric priority setting. </p> <p>You must specify a unique priority for each rule group that you associate with a single VPC. To make it easier to insert rule groups later, leave space between the numbers, for example, use 100, 200, and so on. You can change the priority setting for a rule group association after you create it.</p>\"\n        }\n      ]\n    },\n    \"MutationProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MutationProtectionStatus\"\n        },\n        {\n          \"description\": \"If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\"\
  : \"The name of the rule group association.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FirewallRuleGroupAssociationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-update-firewall-rule-group-association-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: UpdateFirewallRuleGroupAssociationRequest
---
