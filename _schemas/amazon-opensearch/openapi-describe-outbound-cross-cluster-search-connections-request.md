---
description: Container for the parameters to the <code><a>DescribeOutboundCrossClusterSearchConnections</a></code> operation.
layout: schema
name: DescribeOutboundCrossClusterSearchConnectionsRequest
properties_list:
- description: ''
  name: Filters
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-outbound-cross-cluster-search-connections-request-schema.json
slug: openapi-describe-outbound-cross-cluster-search-connections-request
source_filename: openapi-describe-outbound-cross-cluster-search-connections-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-outbound-cross-cluster-search-connections-request-schema.json\",\n  \"title\": \"DescribeOutboundCrossClusterSearchConnectionsRequest\",\n  \"description\": \"Container for the parameters to the <code><a>DescribeOutboundCrossClusterSearchConnections</a></code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \" A list of filters used to match properties for outbound cross-cluster search connection. Available <code><a>Filter</a></code> names for this operation are: <ul> <li>cross-cluster-search-connection-id</li> <li>destination-domain-info.domain-name</li> <li>destination-domain-info.owner-id</li> <li>destination-domain-info.region</li>\
  \ <li>source-domain-info.domain-name</li> </ul> \"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"Set this value to limit the number of results returned. If not specified, defaults to 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" NextToken is sent in case the earlier API call results contain the NextToken. It is used for pagination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-outbound-cross-cluster-search-connections-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DescribeOutboundCrossClusterSearchConnectionsRequest
---
