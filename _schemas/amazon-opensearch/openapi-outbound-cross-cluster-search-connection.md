---
description: Specifies details of an outbound connection.
layout: schema
name: OutboundCrossClusterSearchConnection
properties_list:
- description: ''
  name: SourceDomainInfo
  type: object
- description: ''
  name: DestinationDomainInfo
  type: object
- description: ''
  name: CrossClusterSearchConnectionId
  type: object
- description: ''
  name: ConnectionAlias
  type: object
- description: ''
  name: ConnectionStatus
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-outbound-cross-cluster-search-connection-schema.json
slug: openapi-outbound-cross-cluster-search-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-outbound-cross-cluster-search-connection-schema.json\",\n  \"title\": \"OutboundCrossClusterSearchConnection\",\n  \"description\": \"Specifies details of an outbound connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceDomainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInformation\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>DomainInformation</a></code> for the source Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"DestinationDomainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInformation\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>DomainInformation</a></code> for the destination Elasticsearch domain.\"\n\
  \        }\n      ]\n    },\n    \"CrossClusterSearchConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrossClusterSearchConnectionId\"\n        },\n        {\n          \"description\": \"Specifies the connection id for the outbound cross-cluster search connection.\"\n        }\n      ]\n    },\n    \"ConnectionAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAlias\"\n        },\n        {\n          \"description\": \"Specifies the connection alias for the outbound cross-cluster search connection.\"\n        }\n      ]\n    },\n    \"ConnectionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutboundCrossClusterSearchConnectionStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code><a>OutboundCrossClusterSearchConnectionStatus</a></code> for the outbound connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-outbound-cross-cluster-search-connection-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: OutboundCrossClusterSearchConnection
---
