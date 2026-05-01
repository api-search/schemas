---
description: CreateResolverRuleRequest schema from openapi
layout: schema
name: CreateResolverRuleRequest
properties_list:
- description: ''
  name: CreatorRequestId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RuleType
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: TargetIps
  type: object
- description: ''
  name: ResolverEndpointId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-create-resolver-rule-request-schema.json
slug: amazon-route53-resolver-openapi-create-resolver-rule-request
source_filename: amazon-route53-resolver-openapi-create-resolver-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-rule-request-schema.json\",\n  \"title\": \"CreateResolverRuleRequest\",\n  \"description\": \"CreateResolverRuleRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatorRequestId\"\n        },\n        {\n          \"description\": \"A unique string that identifies the request and that allows failed requests to be retried without the risk of running the operation twice. <code>CreatorRequestId</code> can be any unique string, for example, a date/time stamp. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n         \
  \ \"description\": \"A friendly name that lets you easily find a rule in the Resolver dashboard in the Route 53 console.\"\n        }\n      ]\n    },\n    \"RuleType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleTypeOption\"\n        },\n        {\n          \"description\": \"<p>When you want to forward DNS queries for specified domain name to resolvers on your network, specify <code>FORWARD</code>.</p> <p>When you have a forwarding rule to forward DNS queries for a domain to your network and you want Resolver to process queries for a subdomain of that domain, specify <code>SYSTEM</code>.</p> <p>For example, to forward DNS queries for example.com to resolvers on your network, you create a rule and specify <code>FORWARD</code> for <code>RuleType</code>. To then have Resolver process queries for apex.example.com, you create a rule and specify <code>SYSTEM</code> for <code>RuleType</code>.</p> <p>Currently, only Resolver can create rules that have a\
  \ value of <code>RECURSIVE</code> for <code>RuleType</code>.</p>\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"DNS queries for this domain name are forwarded to the IP addresses that you specify in <code>TargetIps</code>. If a query matches multiple Resolver rules (example.com and www.example.com), outbound DNS queries are routed using the Resolver rule that contains the most specific domain name (www.example.com).\"\n        }\n      ]\n    },\n    \"TargetIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetList\"\n        },\n        {\n          \"description\": \"<p>The IPs that you want Resolver to forward DNS queries to. You can specify only IPv4 addresses. Separate IP addresses with a space.</p> <p> <code>TargetIps</code> is available only when the value of <code>Rule type</code> is <code>FORWARD</code>.</p>\"\
  \n        }\n      ]\n    },\n    \"ResolverEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the outbound Resolver endpoint that you want to use to route DNS queries to the IP addresses that you specify in <code>TargetIps</code>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of the tag keys and values that you want to associate with the endpoint.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatorRequestId\",\n    \"RuleType\",\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-create-resolver-rule-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: CreateResolverRuleRequest
---
