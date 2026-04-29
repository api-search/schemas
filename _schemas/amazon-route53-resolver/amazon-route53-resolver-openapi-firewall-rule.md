---
description: A single firewall rule in a rule group.
layout: schema
name: FirewallRule
properties_list:
- description: ''
  name: FirewallRuleGroupId
  type: object
- description: ''
  name: FirewallDomainListId
  type: object
- description: ''
  name: Name
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
  name: CreatorRequestId
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ModificationTime
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-firewall-rule-schema.json
slug: amazon-route53-resolver-openapi-firewall-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-rule-schema.json\",\n  \"title\": \"FirewallRule\",\n  \"description\": \"A single firewall rule in a rule group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the firewall rule group of the rule. \"\n        }\n      ]\n    },\n    \"FirewallDomainListId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the domain list that's used in the rule. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\
  \n        },\n        {\n          \"description\": \"The name of the rule. \"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"The priority of the rule in the rule group. This value must be unique within the rule group. DNS Firewall processes the rules in a rule group by order of priority, starting from the lowest setting.\"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"<p>The action that DNS Firewall should take on a DNS query when it matches one of the domains in the rule's domain list:</p> <ul> <li> <p> <code>ALLOW</code> - Permit the request to go through.</p> </li> <li> <p> <code>ALERT</code> - Permit the request to go through but send an alert to the logs.</p> </li> <li> <p> <code>BLOCK</code> - Disallow the\
  \ request. If this is specified, additional handling details are provided in the rule's <code>BlockResponse</code> setting. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"BlockResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockResponse\"\n        },\n        {\n          \"description\": \"<p>The way that you want DNS Firewall to block the request. Used for the rule action setting <code>BLOCK</code>.</p> <ul> <li> <p> <code>NODATA</code> - Respond indicating that the query was successful, but no response is available for it.</p> </li> <li> <p> <code>NXDOMAIN</code> - Respond indicating that the domain name that's in the query doesn't exist.</p> </li> <li> <p> <code>OVERRIDE</code> - Provide a custom override in the response. This option requires custom handling details in the rule's <code>BlockOverride*</code> settings. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"BlockOverrideDomain\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/BlockOverrideDomain\"\n        },\n        {\n          \"description\": \"The custom DNS record to send back in response to the query. Used for the rule action <code>BLOCK</code> with a <code>BlockResponse</code> setting of <code>OVERRIDE</code>.\"\n        }\n      ]\n    },\n    \"BlockOverrideDnsType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockOverrideDnsType\"\n        },\n        {\n          \"description\": \"The DNS record's type. This determines the format of the record value that you provided in <code>BlockOverrideDomain</code>. Used for the rule action <code>BLOCK</code> with a <code>BlockResponse</code> setting of <code>OVERRIDE</code>.\"\n        }\n      ]\n    },\n    \"BlockOverrideTtl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Unsigned\"\n        },\n        {\n          \"description\": \"The recommended amount of time, in seconds, for the DNS resolver\
  \ or web browser to cache the provided override record. Used for the rule action <code>BLOCK</code> with a <code>BlockResponse</code> setting of <code>OVERRIDE</code>.\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string defined by you to identify the request. This allows you to retry failed requests without the risk of executing the operation twice. This can be any unique string, for example, a timestamp. \"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the rule was created, in Unix time format and Coordinated Universal Time (UTC). \"\n        }\n      ]\n    },\n    \"ModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the rule was last modified, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-rule-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: FirewallRule
---
