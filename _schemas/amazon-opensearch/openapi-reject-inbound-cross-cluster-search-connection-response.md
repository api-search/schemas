---
description: The result of a <code><a>RejectInboundCrossClusterSearchConnection</a></code> operation. Contains details of rejected inbound connection.
layout: schema
name: RejectInboundCrossClusterSearchConnectionResponse
properties_list:
- description: ''
  name: CrossClusterSearchConnection
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-reject-inbound-cross-cluster-search-connection-response-schema.json
slug: openapi-reject-inbound-cross-cluster-search-connection-response
source_filename: openapi-reject-inbound-cross-cluster-search-connection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-reject-inbound-cross-cluster-search-connection-response-schema.json\",\n  \"title\": \"RejectInboundCrossClusterSearchConnectionResponse\",\n  \"description\": \"The result of a <code><a>RejectInboundCrossClusterSearchConnection</a></code> operation. Contains details of rejected inbound connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrossClusterSearchConnection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InboundCrossClusterSearchConnection\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>InboundCrossClusterSearchConnection</a></code> of rejected inbound connection. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-reject-inbound-cross-cluster-search-connection-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: RejectInboundCrossClusterSearchConnectionResponse
---
