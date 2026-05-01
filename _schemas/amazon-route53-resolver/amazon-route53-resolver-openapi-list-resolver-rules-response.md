---
description: ListResolverRulesResponse schema from openapi
layout: schema
name: ListResolverRulesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: ResolverRules
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-rules-response-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-rules-response
source_filename: amazon-route53-resolver-openapi-list-resolver-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-rules-response-schema.json\",\n  \"title\": \"ListResolverRulesResponse\",\n  \"description\": \"ListResolverRulesResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If more than <code>MaxResults</code> Resolver rules match the specified criteria, you can submit another <code>ListResolverRules</code> request to get the next group of results. In the next request, specify the value of <code>NextToken</code> from the previous response. \"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\
  \n        },\n        {\n          \"description\": \"The value that you specified for <code>MaxResults</code> in the request.\"\n        }\n      ]\n    },\n    \"ResolverRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverRules\"\n        },\n        {\n          \"description\": \"The Resolver rules that were created using the current Amazon Web Services account and that match the specified filters, if any.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-rules-response-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ListResolverRulesResponse
---
