---
description: The result of a <code><a>CreateOutboundCrossClusterSearchConnection</a></code> request. Contains the details of the newly created cross-cluster search connection.
layout: schema
name: CreateOutboundCrossClusterSearchConnectionResponse
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
- description: ''
  name: ConnectionStatus
  type: object
- description: ''
  name: CrossClusterSearchConnectionId
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-outbound-cross-cluster-search-connection-response-schema.json
slug: openapi-create-outbound-cross-cluster-search-connection-response
source_filename: openapi-create-outbound-cross-cluster-search-connection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-outbound-cross-cluster-search-connection-response-schema.json\",\n  \"title\": \"CreateOutboundCrossClusterSearchConnectionResponse\",\n  \"description\": \"The result of a <code><a>CreateOutboundCrossClusterSearchConnection</a></code> request. Contains the details of the newly created cross-cluster search connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceDomainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInformation\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>DomainInformation</a></code> for the source Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"DestinationDomainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInformation\"\n\
  \        },\n        {\n          \"description\": \"Specifies the <code><a>DomainInformation</a></code> for the destination Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"ConnectionAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAlias\"\n        },\n        {\n          \"description\": \"Specifies the connection alias provided during the create connection request.\"\n        }\n      ]\n    },\n    \"ConnectionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutboundCrossClusterSearchConnectionStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>OutboundCrossClusterSearchConnectionStatus</a></code> for the newly created connection.\"\n        }\n      ]\n    },\n    \"CrossClusterSearchConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrossClusterSearchConnectionId\"\n        },\n        {\n          \"description\"\
  : \"Unique id for the created outbound connection, which is used for subsequent operations on connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-outbound-cross-cluster-search-connection-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CreateOutboundCrossClusterSearchConnectionResponse
---
