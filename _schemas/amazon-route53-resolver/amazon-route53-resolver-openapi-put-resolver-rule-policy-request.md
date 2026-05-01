---
description: PutResolverRulePolicyRequest schema from openapi
layout: schema
name: PutResolverRulePolicyRequest
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: ResolverRulePolicy
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-put-resolver-rule-policy-request-schema.json
slug: amazon-route53-resolver-openapi-put-resolver-rule-policy-request
source_filename: amazon-route53-resolver-openapi-put-resolver-rule-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-rule-policy-request-schema.json\",\n  \"title\": \"PutResolverRulePolicyRequest\",\n  \"description\": \"PutResolverRulePolicyRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the rule that you want to share with another account.\"\n        }\n      ]\n    },\n    \"ResolverRulePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRulePolicy\"\n        },\n        {\n          \"description\": \"<p>An Identity and Access Management policy statement that lists the rules that you want to share with another\
  \ Amazon Web Services account and the operations that you want the account to be able to perform. You can specify the following operations in the <code>Action</code> section of the statement:</p> <ul> <li> <p> <code>route53resolver:GetResolverRule</code> </p> </li> <li> <p> <code>route53resolver:AssociateResolverRule</code> </p> </li> <li> <p> <code>route53resolver:DisassociateResolverRule</code> </p> </li> <li> <p> <code>route53resolver:ListResolverRules</code> </p> </li> <li> <p> <code>route53resolver:ListResolverRuleAssociations</code> </p> </li> </ul> <p>In the <code>Resource</code> section of the statement, specify the ARN for the rule that you want to share with another account. Specify the same ARN that you specified in <code>Arn</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"ResolverRulePolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-rule-policy-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: PutResolverRulePolicyRequest
---
