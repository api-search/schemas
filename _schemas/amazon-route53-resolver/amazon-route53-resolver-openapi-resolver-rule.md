---
description: For queries that originate in your VPC, detailed information about a Resolver rule, which specifies how to route DNS queries out of the VPC. The <code>ResolverRule</code> parameter appears in the response to a <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverRule.html">CreateResolverRule</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DeleteResolverRule.html">DeleteResolverRule</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverRule.html">GetResolverRule</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverRules.html">ListResolverRules</a>, or <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverRule.html">UpdateResolverRule</a> request.
layout: schema
name: ResolverRule
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: RuleType
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: TargetIps
  type: object
- description: ''
  name: ResolverEndpointId
  type: object
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: ShareStatus
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ModificationTime
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-rule-schema.json
slug: amazon-route53-resolver-openapi-resolver-rule
source_filename: amazon-route53-resolver-openapi-resolver-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-rule-schema.json\",\n  \"title\": \"ResolverRule\",\n  \"description\": \"For queries that originate in your VPC, detailed information about a Resolver rule, which specifies how to route DNS queries out of the VPC. The <code>ResolverRule</code> parameter appears in the response to a <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_CreateResolverRule.html\\\">CreateResolverRule</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DeleteResolverRule.html\\\">DeleteResolverRule</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverRule.html\\\">GetResolverRule</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverRules.html\\\
  \">ListResolverRules</a>, or <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_UpdateResolverRule.html\\\">UpdateResolverRule</a> request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID that Resolver assigned to the Resolver rule when you created it.\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that you specified when you created the Resolver rule. <code>CreatorRequestId</code> identifies the request and allows failed requests to be retried without the risk of running the operation twice. \"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\
  \n        },\n        {\n          \"description\": \"The ARN (Amazon Resource Name) for the Resolver rule specified by <code>Id</code>.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"DNS queries for this domain name are forwarded to the IP addresses that are specified in <code>TargetIps</code>. If a query matches multiple Resolver rules (example.com and www.example.com), the query is routed using the Resolver rule that contains the most specific domain name (www.example.com).\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRuleStatus\"\n        },\n        {\n          \"description\": \"A code that specifies the current status of the Resolver rule.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"A detailed description of the status of a Resolver rule.\"\n        }\n      ]\n    },\n    \"RuleType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleTypeOption\"\n        },\n        {\n          \"description\": \"<p>When you want to forward DNS queries for specified domain name to resolvers on your network, specify <code>FORWARD</code>.</p> <p>When you have a forwarding rule to forward DNS queries for a domain to your network and you want Resolver to process queries for a subdomain of that domain, specify <code>SYSTEM</code>.</p> <p>For example, to forward DNS queries for example.com to resolvers on your network, you create a rule and specify <code>FORWARD</code> for <code>RuleType</code>. To then have Resolver process queries for apex.example.com, you create a rule and specify <code>SYSTEM</code> for <code>RuleType</code>.</p> <p>Currently, only Resolver can\
  \ create rules that have a value of <code>RECURSIVE</code> for <code>RuleType</code>.</p>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name for the Resolver rule, which you specified when you created the Resolver rule.\"\n        }\n      ]\n    },\n    \"TargetIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetList\"\n        },\n        {\n          \"description\": \"An array that contains the IP addresses and ports that an outbound endpoint forwards DNS queries to. Typically, these are the IP addresses of DNS resolvers on your network. Specify IPv4 addresses. IPv6 is not supported.\"\n        }\n      ]\n    },\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the endpoint that\
  \ the rule is associated with.\"\n        }\n      ]\n    },\n    \"OwnerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"When a rule is shared with another Amazon Web Services account, the account ID of the account that the rule is shared with.\"\n        }\n      ]\n    },\n    \"ShareStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareStatus\"\n        },\n        {\n          \"description\": \"Whether the rule is shared and, if so, whether the current account is sharing the rule with another account, or another account is sharing the rule with the current account.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the Resolver rule was created, in Unix time format and Coordinated\
  \ Universal Time (UTC).\"\n        }\n      ]\n    },\n    \"ModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the Resolver rule was last updated, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-rule-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ResolverRule
---
