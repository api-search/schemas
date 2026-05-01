---
description: Container for the parameters to the <code><a>CreateOutboundCrossClusterSearchConnection</a></code> operation.
layout: schema
name: CreateOutboundCrossClusterSearchConnectionRequest
properties_list:
- description: ''
  name: SourceDomainInfo
  type: object
- description: ''
  name: DestinationDomainInfo
  type: object
- description: ''
  name: ConnectionAlias
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-outbound-cross-cluster-search-connection-request-schema.json
slug: openapi-create-outbound-cross-cluster-search-connection-request
source_filename: openapi-create-outbound-cross-cluster-search-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-outbound-cross-cluster-search-connection-request-schema.json\",\n  \"title\": \"CreateOutboundCrossClusterSearchConnectionRequest\",\n  \"description\": \"Container for the parameters to the <code><a>CreateOutboundCrossClusterSearchConnection</a></code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceDomainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInformation\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>DomainInformation</a></code> for the source Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"DestinationDomainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInformation\"\n        },\n        {\n          \"description\": \"Specifies\
  \ the <code><a>DomainInformation</a></code> for the destination Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"ConnectionAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAlias\"\n        },\n        {\n          \"description\": \"Specifies the connection alias that will be used by the customer for this connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceDomainInfo\",\n    \"DestinationDomainInfo\",\n    \"ConnectionAlias\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-outbound-cross-cluster-search-connection-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: CreateOutboundCrossClusterSearchConnectionRequest
---
