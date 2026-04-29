---
description: ListResolverDnssecConfigsResponse schema from openapi
layout: schema
name: ListResolverDnssecConfigsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ResolverDnssecConfigs
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-dnssec-configs-response-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-dnssec-configs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-dnssec-configs-response-schema.json\",\n  \"title\": \"ListResolverDnssecConfigsResponse\",\n  \"description\": \"ListResolverDnssecConfigsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>If a response includes the last of the DNSSEC configurations that are associated with the current Amazon Web Services account, <code>NextToken</code> doesn't appear in the response.</p> <p>If a response doesn't include the last of the configurations, you can get more configurations by submitting another <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_ListResolverDnssecConfigs.html\\\
  \">ListResolverDnssecConfigs</a> request. Get the value of <code>NextToken</code> that Amazon Route 53 returned in the previous response and include it in <code>NextToken</code> in the next request.</p>\"\n        }\n      ]\n    },\n    \"ResolverDnssecConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverDnssecConfigList\"\n        },\n        {\n          \"description\": \"An array that contains one <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_ResolverDnssecConfig.html\\\">ResolverDnssecConfig</a> element for each configuration for DNSSEC validation that is associated with the current Amazon Web Services account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-dnssec-configs-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListResolverDnssecConfigsResponse
---
