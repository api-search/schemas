---
description: ListResolverQueryLogConfigAssociationsResponse schema from openapi
layout: schema
name: ListResolverQueryLogConfigAssociationsResponse
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
  name: ResolverQueryLogConfigAssociations
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-response-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-response-schema.json\",\n  \"title\": \"ListResolverQueryLogConfigAssociationsResponse\",\n  \"description\": \"ListResolverQueryLogConfigAssociationsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If there are more than <code>MaxResults</code> query logging associations, you can submit another <code>ListResolverQueryLogConfigAssociations</code> request to get the next group of associations. In the next request, specify the value of <code>NextToken</code> from the previous response. \"\n        }\n      ]\n    },\n    \"TotalCount\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The total number of query logging associations that were created by the current account in the specified Region. This count can differ from the number of associations that are returned in a <code>ListResolverQueryLogConfigAssociations</code> response, depending on the values that you specify in the request.\"\n        }\n      ]\n    },\n    \"TotalFilteredCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The total number of query logging associations that were created by the current account in the specified Region and that match the filters that were specified in the <code>ListResolverQueryLogConfigAssociations</code> request. For the total number of associations that were created by the current account in the specified Region, see <code>TotalCount</code>.\"\
  \n        }\n      ]\n    },\n    \"ResolverQueryLogConfigAssociations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigAssociationList\"\n        },\n        {\n          \"description\": \"A list that contains one <code>ResolverQueryLogConfigAssociations</code> element for each query logging association that matches the values that you specified for <code>Filter</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverQueryLogConfigAssociationsResponse
---
