---
description: ListResolverQueryLogConfigsResponse schema from openapi
layout: schema
name: ListResolverQueryLogConfigsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: TotalCount
  type: object
- description: ''
  name: TotalFilteredCount
  type: object
- description: ''
  name: ResolverQueryLogConfigs
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-configs-response-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-query-log-configs-response
source_filename: amazon-route53-resolver-openapi-list-resolver-query-log-configs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-configs-response-schema.json\",\n  \"title\": \"ListResolverQueryLogConfigsResponse\",\n  \"description\": \"ListResolverQueryLogConfigsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If there are more than <code>MaxResults</code> query logging configurations, you can submit another <code>ListResolverQueryLogConfigs</code> request to get the next group of configurations. In the next request, specify the value of <code>NextToken</code> from the previous response. \"\n        }\n      ]\n    },\n    \"TotalCount\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The total number of query logging configurations that were created by the current account in the specified Region. This count can differ from the number of query logging configurations that are returned in a <code>ListResolverQueryLogConfigs</code> response, depending on the values that you specify in the request.\"\n        }\n      ]\n    },\n    \"TotalFilteredCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The total number of query logging configurations that were created by the current account in the specified Region and that match the filters that were specified in the <code>ListResolverQueryLogConfigs</code> request. For the total number of query logging configurations that were created by the current account in the specified Region, see <code>TotalCount</code>.\"\n        }\n    \
  \  ]\n    },\n    \"ResolverQueryLogConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigList\"\n        },\n        {\n          \"description\": \"A list that contains one <code>ResolverQueryLogConfig</code> element for each query logging configuration that matches the values that you specified for <code>Filter</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-configs-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverQueryLogConfigsResponse
---
