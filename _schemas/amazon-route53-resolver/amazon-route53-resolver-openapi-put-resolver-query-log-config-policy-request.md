---
description: PutResolverQueryLogConfigPolicyRequest schema from openapi
layout: schema
name: PutResolverQueryLogConfigPolicyRequest
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: ResolverQueryLogConfigPolicy
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-request-schema.json
slug: amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-request-schema.json\",\n  \"title\": \"PutResolverQueryLogConfigPolicyRequest\",\n  \"description\": \"PutResolverQueryLogConfigPolicyRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the account that you want to share rules with.\"\n        }\n      ]\n    },\n    \"ResolverQueryLogConfigPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigPolicy\"\n        },\n        {\n          \"description\": \"<p>An Identity and Access Management policy statement that lists\
  \ the query logging configurations that you want to share with another Amazon Web Services account and the operations that you want the account to be able to perform. You can specify the following operations in the <code>Actions</code> section of the statement:</p> <ul> <li> <p> <code>route53resolver:AssociateResolverQueryLogConfig</code> </p> </li> <li> <p> <code>route53resolver:DisassociateResolverQueryLogConfig</code> </p> </li> <li> <p> <code>route53resolver:ListResolverQueryLogConfigAssociations</code> </p> </li> <li> <p> <code>route53resolver:ListResolverQueryLogConfigs</code> </p> </li> </ul> <p>In the <code>Resource</code> section of the statement, you specify the ARNs for the query logging configurations that you want to share with the account that you specified in <code>Arn</code>. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"ResolverQueryLogConfigPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-put-resolver-query-log-config-policy-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: PutResolverQueryLogConfigPolicyRequest
---
