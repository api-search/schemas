---
description: GetAggregateDiscoveredResourceCountsResponse schema
layout: schema
name: GetAggregateDiscoveredResourceCountsResponse
properties_list:
- description: ''
  name: TotalDiscoveredResources
  type: object
- description: ''
  name: GroupByKey
  type: object
- description: ''
  name: GroupedResourceCounts
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-discovered-resource-counts-response-schema.json
slug: config-get-aggregate-discovered-resource-counts-response
source_filename: config-get-aggregate-discovered-resource-counts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-discovered-resource-counts-response-schema.json\",\n  \"title\": \"GetAggregateDiscoveredResourceCountsResponse\",\n  \"description\": \"GetAggregateDiscoveredResourceCountsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalDiscoveredResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total number of resources that are present in an aggregator with the filters that you provide.\"\n        }\n      ]\n    },\n    \"GroupByKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The key passed into the request object. If <code>GroupByKey</code> is not provided,\
  \ the result will be empty.\"\n        }\n      ]\n    },\n    \"GroupedResourceCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupedResourceCountList\"\n        },\n        {\n          \"description\": \"Returns a list of GroupedResourceCount objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TotalDiscoveredResources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-discovered-resource-counts-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateDiscoveredResourceCountsResponse
---
