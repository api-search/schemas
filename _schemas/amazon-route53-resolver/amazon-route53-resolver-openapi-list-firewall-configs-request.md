---
description: ListFirewallConfigsRequest schema from openapi
layout: schema
name: ListFirewallConfigsRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-firewall-configs-request-schema.json
slug: amazon-route53-resolver-openapi-list-firewall-configs-request
source_filename: amazon-route53-resolver-openapi-list-firewall-configs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-firewall-configs-request-schema.json\",\n  \"title\": \"ListFirewallConfigsRequest\",\n  \"description\": \"ListFirewallConfigsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListFirewallConfigsMaxResult\"\n        },\n        {\n          \"description\": \"<p>The maximum number of objects that you want Resolver to return for this request. If more objects are available, in the response, Resolver provides a <code>NextToken</code> value that you can use in a subsequent call to get the next batch of objects.</p> <p>If you don't specify a value for <code>MaxResults</code>, Resolver returns up to 100 objects. </p>\"\n        }\n      ]\n\
  \    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>For the first call to this list request, omit this value.</p> <p>When you request a list of objects, Resolver returns at most the number of objects specified in <code>MaxResults</code>. If more objects are available for retrieval, Resolver returns a <code>NextToken</code> value in the response. To retrieve the next batch of objects, use the token that was returned for the prior request in your next request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-firewall-configs-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ListFirewallConfigsRequest
---
