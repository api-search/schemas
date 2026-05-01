---
description: ListTagsForResourceRequest schema from openapi
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-tags-for-resource-request-schema.json
slug: amazon-route53-resolver-openapi-list-tags-for-resource-request
source_filename: amazon-route53-resolver-openapi-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the resource that you want to list tags for.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of tags that you want to return in the response to a <code>ListTagsForResource</code> request. If you don't specify\
  \ a value for <code>MaxResults</code>, Resolver returns up to 100 tags.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>For the first <code>ListTagsForResource</code> request, omit this value.</p> <p>If you have more than <code>MaxResults</code> tags, you can submit another <code>ListTagsForResource</code> request to get the next group of tags for the resource. In the next request, specify the value of <code>NextToken</code> from the previous response. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-tags-for-resource-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ListTagsForResourceRequest
---
