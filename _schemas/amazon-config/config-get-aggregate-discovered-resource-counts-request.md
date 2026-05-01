---
description: GetAggregateDiscoveredResourceCountsRequest schema
layout: schema
name: GetAggregateDiscoveredResourceCountsRequest
properties_list:
- description: ''
  name: ConfigurationAggregatorName
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: GroupByKey
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-aggregate-discovered-resource-counts-request-schema.json
slug: config-get-aggregate-discovered-resource-counts-request
source_filename: config-get-aggregate-discovered-resource-counts-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-discovered-resource-counts-request-schema.json\",\n  \"title\": \"GetAggregateDiscoveredResourceCountsRequest\",\n  \"description\": \"GetAggregateDiscoveredResourceCountsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationAggregatorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationAggregatorName\"\n        },\n        {\n          \"description\": \"The name of the configuration aggregator.\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountFilters\"\n        },\n        {\n          \"description\": \"Filters the results based on the <code>ResourceCountFilters</code> object.\"\n        }\n      ]\n    },\n    \"GroupByKey\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountGroupKey\"\n        },\n        {\n          \"description\": \"The key to group the resource counts.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupByAPILimit\"\n        },\n        {\n          \"description\": \"The maximum number of <a>GroupedResourceCount</a> objects returned on each page. The default is 1000. You cannot specify a number greater than 1000. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationAggregatorName\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-aggregate-discovered-resource-counts-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetAggregateDiscoveredResourceCountsRequest
---
