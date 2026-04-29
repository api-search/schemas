---
description: ListTagsForResourceResponse schema from openapi
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: Tags
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-tags-for-resource-response-schema.json
slug: amazon-route53-resolver-openapi-list-tags-for-resource-response
source_filename: amazon-route53-resolver-openapi-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags that are associated with the resource that you specified in the <code>ListTagsForResource</code> request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If more than <code>MaxResults</code> tags match the specified criteria, you can submit another <code>ListTagsForResource</code>\
  \ request to get the next group of results. In the next request, specify the value of <code>NextToken</code> from the previous response. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-tags-for-resource-response-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListTagsForResourceResponse
---
