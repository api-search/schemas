---
description: ListResolverConfigsRequest schema from openapi
layout: schema
name: ListResolverConfigsRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-configs-request-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-configs-request
source_filename: amazon-route53-resolver-openapi-list-resolver-configs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-configs-request-schema.json\",\n  \"title\": \"ListResolverConfigsRequest\",\n  \"description\": \"ListResolverConfigsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListResolverConfigsMaxResult\"\n        },\n        {\n          \"description\": \"The maximum number of Resolver configurations that you want to return in the response to a <code>ListResolverConfigs</code> request. If you don't specify a value for <code>MaxResults</code>, up to 100 Resolver configurations are returned.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n  \
  \      },\n        {\n          \"description\": \"<p>(Optional) If the current Amazon Web Services account has more than <code>MaxResults</code> Resolver configurations, use <code>NextToken</code> to get the second and subsequent pages of results.</p> <p>For the first <code>ListResolverConfigs</code> request, omit this value.</p> <p>For the second and subsequent requests, get the value of <code>NextToken</code> from the previous response and specify that value for <code>NextToken</code> in the request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-configs-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ListResolverConfigsRequest
---
