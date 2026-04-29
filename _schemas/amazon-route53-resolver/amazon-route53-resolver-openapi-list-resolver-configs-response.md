---
description: ListResolverConfigsResponse schema from openapi
layout: schema
name: ListResolverConfigsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ResolverConfigs
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-configs-response-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-configs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-configs-response-schema.json\",\n  \"title\": \"ListResolverConfigsResponse\",\n  \"description\": \"ListResolverConfigsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>If a response includes the last of the Resolver configurations that are associated with the current Amazon Web Services account, <code>NextToken</code> doesn't appear in the response.</p> <p>If a response doesn't include the last of the configurations, you can get more configurations by submitting another <code>ListResolverConfigs</code> request. Get the value of <code>NextToken</code> that Amazon\
  \ Route\\u00a053 returned in the previous response and include it in <code>NextToken</code> in the next request.</p>\"\n        }\n      ]\n    },\n    \"ResolverConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverConfigList\"\n        },\n        {\n          \"description\": \"An array that contains one <code>ResolverConfigs</code> element for each Resolver configuration that is associated with the current Amazon Web Services account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-configs-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverConfigsResponse
---
