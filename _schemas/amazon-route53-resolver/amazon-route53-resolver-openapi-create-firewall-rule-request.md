---
description: CreateFirewallRuleRequest schema from openapi
layout: schema
name: CreateFirewallRuleRequest
properties_list:
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: FirewallRuleGroupId
  type: object
- description: ''
  name: FirewallDomainListId
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: BlockResponse
  type: object
- description: ''
  name: BlockOverrideDomain
  type: object
- description: ''
  name: BlockOverrideDnsType
  type: object
- description: ''
  name: BlockOverrideTtl
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-firewall-rule-request-schema.json
slug: amazon-route53-resolver-openapi-create-firewall-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-firewall-rule-request-schema.json\",\n  \"title\": \"CreateFirewallRuleRequest\",\n  \"description\": \"CreateFirewallRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request and that allows you to retry failed requests without the risk of running the operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. \"\n        }\n      ]\n    },\n    \"FirewallRuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n\
  \        {\n          \"description\": \"The unique identifier of the firewall rule group where you want to create the rule. \"\n        }\n      ]\n    },\n    \"FirewallDomainListId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list that you want to use in the rule. \"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"<p>The setting that determines the processing order of the rule in the rule group. DNS Firewall processes the rules in a rule group by order of priority, starting from the lowest setting.</p> <p>You must specify a unique priority for each rule in a rule group. To make it easier to insert rules later, leave space between the numbers, for example, use 100, 200, and so on. You can change the priority setting for the rules\
  \ in a rule group at any time.</p>\"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"<p>The action that DNS Firewall should take on a DNS query when it matches one of the domains in the rule's domain list:</p> <ul> <li> <p> <code>ALLOW</code> - Permit the request to go through.</p> </li> <li> <p> <code>ALERT</code> - Permit the request and send metrics and logs to Cloud Watch.</p> </li> <li> <p> <code>BLOCK</code> - Disallow the request. This option requires additional details in the rule's <code>BlockResponse</code>. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"BlockResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockResponse\"\n        },\n        {\n          \"description\": \"<p>The way that you want DNS Firewall to block the request, used with the rule action setting <code>BLOCK</code>. </p> <ul>\
  \ <li> <p> <code>NODATA</code> - Respond indicating that the query was successful, but no response is available for it.</p> </li> <li> <p> <code>NXDOMAIN</code> - Respond indicating that the domain name that's in the query doesn't exist.</p> </li> <li> <p> <code>OVERRIDE</code> - Provide a custom override in the response. This option requires custom handling details in the rule's <code>BlockOverride*</code> settings. </p> </li> </ul> <p>This setting is required if the rule action setting is <code>BLOCK</code>.</p>\"\n        }\n      ]\n    },\n    \"BlockOverrideDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockOverrideDomain\"\n        },\n        {\n          \"description\": \"<p>The custom DNS record to send back in response to the query. Used for the rule action <code>BLOCK</code> with a <code>BlockResponse</code> setting of <code>OVERRIDE</code>.</p> <p>This setting is required if the <code>BlockResponse</code> setting is <code>OVERRIDE</code>.</p>\"\
  \n        }\n      ]\n    },\n    \"BlockOverrideDnsType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockOverrideDnsType\"\n        },\n        {\n          \"description\": \"<p>The DNS record's type. This determines the format of the record value that you provided in <code>BlockOverrideDomain</code>. Used for the rule action <code>BLOCK</code> with a <code>BlockResponse</code> setting of <code>OVERRIDE</code>.</p> <p>This setting is required if the <code>BlockResponse</code> setting is <code>OVERRIDE</code>.</p>\"\n        }\n      ]\n    },\n    \"BlockOverrideTtl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockOverrideTtl\"\n        },\n        {\n          \"description\": \"<p>The recommended amount of time, in seconds, for the DNS resolver or web browser to cache the provided override record. Used for the rule action <code>BLOCK</code> with a <code>BlockResponse</code> setting of <code>OVERRIDE</code>.</p>\
  \ <p>This setting is required if the <code>BlockResponse</code> setting is <code>OVERRIDE</code>.</p>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"A name that lets you identify the rule in the rule group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatorRequestId\",\n    \"FirewallRuleGroupId\",\n    \"FirewallDomainListId\",\n    \"Priority\",\n    \"Action\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-firewall-rule-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: CreateFirewallRuleRequest
---
