---
description: ListResolverRulesRequest schema from openapi
layout: schema
name: ListResolverRulesRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Filters
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-rules-request-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-rules-request
source_filename: amazon-route53-resolver-openapi-list-resolver-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-rules-request-schema.json\",\n  \"title\": \"ListResolverRulesRequest\",\n  \"description\": \"ListResolverRulesRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of Resolver rules that you want to return in the response to a <code>ListResolverRules</code> request. If you don't specify a value for <code>MaxResults</code>, Resolver returns up to 100 Resolver rules.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\"\
  : \"<p>For the first <code>ListResolverRules</code> request, omit this value.</p> <p>If you have more than <code>MaxResults</code> Resolver rules, you can submit another <code>ListResolverRules</code> request to get the next group of Resolver rules. In the next request, specify the value of <code>NextToken</code> from the previous response. </p>\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"<p>An optional specification to return a subset of Resolver rules, such as all Resolver rules that are associated with the same Resolver endpoint.</p> <note> <p>If you submit a second or subsequent <code>ListResolverRules</code> request and specify the <code>NextToken</code> parameter, you must use the same values for <code>Filters</code>, if any, as in the previous request.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-rules-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverRulesRequest
---
