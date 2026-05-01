---
description: The result of a <code><a>DeleteInboundCrossClusterSearchConnection</a></code> operation. Contains details of deleted inbound connection.
layout: schema
name: DeleteInboundCrossClusterSearchConnectionResponse
properties_list:
- description: ''
  name: CrossClusterSearchConnection
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-delete-inbound-cross-cluster-search-connection-response-schema.json
slug: openapi-delete-inbound-cross-cluster-search-connection-response
source_filename: openapi-delete-inbound-cross-cluster-search-connection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-inbound-cross-cluster-search-connection-response-schema.json\",\n  \"title\": \"DeleteInboundCrossClusterSearchConnectionResponse\",\n  \"description\": \"The result of a <code><a>DeleteInboundCrossClusterSearchConnection</a></code> operation. Contains details of deleted inbound connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrossClusterSearchConnection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InboundCrossClusterSearchConnection\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>InboundCrossClusterSearchConnection</a></code> of deleted inbound connection. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-inbound-cross-cluster-search-connection-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DeleteInboundCrossClusterSearchConnectionResponse
---
