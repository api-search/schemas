---
description: The result of a <code><a>AcceptInboundCrossClusterSearchConnection</a></code> operation. Contains details of accepted inbound connection.
layout: schema
name: AcceptInboundCrossClusterSearchConnectionResponse
properties_list:
- description: ''
  name: CrossClusterSearchConnection
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-accept-inbound-cross-cluster-search-connection-response-schema.json
slug: openapi-accept-inbound-cross-cluster-search-connection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-accept-inbound-cross-cluster-search-connection-response-schema.json\",\n  \"title\": \"AcceptInboundCrossClusterSearchConnectionResponse\",\n  \"description\": \"The result of a <code><a>AcceptInboundCrossClusterSearchConnection</a></code> operation. Contains details of accepted inbound connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrossClusterSearchConnection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InboundCrossClusterSearchConnection\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>InboundCrossClusterSearchConnection</a></code> of accepted inbound connection. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-accept-inbound-cross-cluster-search-connection-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AcceptInboundCrossClusterSearchConnectionResponse
---
