---
description: The result of a <code><a>DescribeOutboundCrossClusterSearchConnections</a></code> request. Contains the list of connections matching the filter criteria.
layout: schema
name: DescribeOutboundCrossClusterSearchConnectionsResponse
properties_list:
- description: ''
  name: CrossClusterSearchConnections
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-outbound-cross-cluster-search-connections-response-schema.json
slug: openapi-describe-outbound-cross-cluster-search-connections-response
source_filename: openapi-describe-outbound-cross-cluster-search-connections-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-outbound-cross-cluster-search-connections-response-schema.json\",\n  \"title\": \"DescribeOutboundCrossClusterSearchConnectionsResponse\",\n  \"description\": \"The result of a <code><a>DescribeOutboundCrossClusterSearchConnections</a></code> request. Contains the list of connections matching the filter criteria.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrossClusterSearchConnections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutboundCrossClusterSearchConnections\"\n        },\n        {\n          \"description\": \"Consists of list of <code><a>OutboundCrossClusterSearchConnection</a></code> matching the specified filter criteria.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If more results are available and NextToken is present, make the next request to the same API with the received NextToken to paginate the remaining results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-outbound-cross-cluster-search-connections-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DescribeOutboundCrossClusterSearchConnectionsResponse
---
