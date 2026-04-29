---
description: ListTagsForResourceRequest schema from Amazon Network Firewall
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-list-tags-for-resource-request-schema.json
slug: openapi-list-tags-for-resource-request
source_filename: openapi-list-tags-for-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-tags-for-resource-request-schema.json\",\n  \"title\": \"ListTagsForResourceRequest\",\n  \"description\": \"ListTagsForResourceRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"When you request a list of objects with a <code>MaxResults</code> setting, if the number of objects that are still available for retrieval exceeds the maximum you requested, Network Firewall returns a <code>NextToken</code> value in the response. To retrieve the next batch of objects, use the token returned from the prior request in your next request.\"\n        }\n      ]\n    },\n    \"MaxResults\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsPaginationMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of objects that you want Network Firewall to return for this request. If more objects are available, in the response, Network Firewall provides a <code>NextToken</code> value that you can use in a subsequent call to get the next batch of objects.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-list-tags-for-resource-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ListTagsForResourceRequest
---
