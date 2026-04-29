---
description: The result of a <code><a>DeleteOutboundCrossClusterSearchConnection</a></code> operation. Contains details of deleted outbound connection.
layout: schema
name: DeleteOutboundCrossClusterSearchConnectionResponse
properties_list:
- description: ''
  name: CrossClusterSearchConnection
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-delete-outbound-cross-cluster-search-connection-response-schema.json
slug: openapi-delete-outbound-cross-cluster-search-connection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-outbound-cross-cluster-search-connection-response-schema.json\",\n  \"title\": \"DeleteOutboundCrossClusterSearchConnectionResponse\",\n  \"description\": \"The result of a <code><a>DeleteOutboundCrossClusterSearchConnection</a></code> operation. Contains details of deleted outbound connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrossClusterSearchConnection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutboundCrossClusterSearchConnection\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>OutboundCrossClusterSearchConnection</a></code> of deleted outbound connection. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-outbound-cross-cluster-search-connection-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DeleteOutboundCrossClusterSearchConnectionResponse
---
