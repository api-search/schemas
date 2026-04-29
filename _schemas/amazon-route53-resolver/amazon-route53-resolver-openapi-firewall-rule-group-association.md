---
description: An association between a firewall rule group and a VPC, which enables DNS filtering for the VPC.
layout: schema
name: FirewallRuleGroupAssociation
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: FirewallRuleGroupId
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: MutationProtection
  type: object
- description: ''
  name: ManagedOwnerName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
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
schema_file: json-schema/amazon-route53-resolver-openapi-firewall-rule-group-association-schema.json
slug: amazon-route53-resolver-openapi-firewall-rule-group-association
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-rule-group-association-schema.json\",\n  \"title\": \"FirewallRuleGroupAssociation\",\n  \"description\": \"An association between a firewall rule group and a VPC, which enables DNS filtering for the VPC. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for the association.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the firewall rule group association.\"\n        }\n      ]\n    },\n    \"FirewallRuleGroupId\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the firewall rule group. \"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the VPC that is associated with the rule group. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the association.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"The setting that determines the processing order of the rule group among the rule groups that are associated with a single VPC. DNS Firewall filters\
  \ VPC traffic starting from rule group with the lowest numeric priority setting. \"\n        }\n      ]\n    },\n    \"MutationProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MutationProtectionStatus\"\n        },\n        {\n          \"description\": \"If enabled, this setting disallows modification or removal of the association, to help prevent against accidentally altering DNS firewall protections. \"\n        }\n      ]\n    },\n    \"ManagedOwnerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServicePrinciple\"\n        },\n        {\n          \"description\": \"The owner of the association, used only for associations that are not managed by you. If you use Firewall Manager to manage your DNS Firewalls, then this reports Firewall Manager as the managed owner.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroupAssociationStatus\"\
  \n        },\n        {\n          \"description\": \"The current status of the association.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"Additional information about the status of the response, if available.\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string defined by you to identify the request. This allows you to retry failed requests without the risk of running the operation twice. This can be any unique string, for example, a timestamp. \"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that\
  \ the association was created, in Unix time format and Coordinated Universal Time (UTC). \"\n        }\n      ]\n    },\n    \"ModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the association was last modified, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-firewall-rule-group-association-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: FirewallRuleGroupAssociation
---
