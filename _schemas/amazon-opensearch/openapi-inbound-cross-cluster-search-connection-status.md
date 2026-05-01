---
description: Specifies the coonection status of an inbound cross-cluster search connection.
layout: schema
name: InboundCrossClusterSearchConnectionStatus
properties_list:
- description: ''
  name: StatusCode
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-inbound-cross-cluster-search-connection-status-schema.json
slug: openapi-inbound-cross-cluster-search-connection-status
source_filename: openapi-inbound-cross-cluster-search-connection-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-inbound-cross-cluster-search-connection-status-schema.json\",\n  \"title\": \"InboundCrossClusterSearchConnectionStatus\",\n  \"description\": \"Specifies the coonection status of an inbound cross-cluster search connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StatusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InboundCrossClusterSearchConnectionStatusCode\"\n        },\n        {\n          \"description\": \"<p>The state code for inbound connection. This can be one of the following:</p> <ul> <li>PENDING_ACCEPTANCE: Inbound connection is not yet accepted by destination domain owner.</li> <li>APPROVED: Inbound connection is pending acceptance by destination domain owner.</li> <li>REJECTING: Inbound connection rejection is in process.</li>\
  \ <li>REJECTED: Inbound connection is rejected.</li> <li>DELETING: Inbound connection deletion is in progress.</li> <li>DELETED: Inbound connection is deleted and cannot be used further.</li> </ul>\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrossClusterSearchConnectionStatusMessage\"\n        },\n        {\n          \"description\": \"Specifies verbose information for the inbound connection status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-inbound-cross-cluster-search-connection-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: InboundCrossClusterSearchConnectionStatus
---
