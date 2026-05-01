---
description: Specifies the connection status of an outbound cross-cluster search connection.
layout: schema
name: OutboundCrossClusterSearchConnectionStatus
properties_list:
- description: ''
  name: StatusCode
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-outbound-cross-cluster-search-connection-status-schema.json
slug: openapi-outbound-cross-cluster-search-connection-status
source_filename: openapi-outbound-cross-cluster-search-connection-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-outbound-cross-cluster-search-connection-status-schema.json\",\n  \"title\": \"OutboundCrossClusterSearchConnectionStatus\",\n  \"description\": \"Specifies the connection status of an outbound cross-cluster search connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StatusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutboundCrossClusterSearchConnectionStatusCode\"\n        },\n        {\n          \"description\": \"<p>The state code for outbound connection. This can be one of the following:</p> <ul> <li>VALIDATING: The outbound connection request is being validated.</li> <li>VALIDATION_FAILED: Validation failed for the connection request.</li> <li>PENDING_ACCEPTANCE: Outbound connection request is validated and is not yet accepted by destination\
  \ domain owner.</li> <li>PROVISIONING: Outbound connection request is in process.</li> <li>ACTIVE: Outbound connection is active and ready to use.</li> <li>REJECTED: Outbound connection request is rejected by destination domain owner.</li> <li>DELETING: Outbound connection deletion is in progress.</li> <li>DELETED: Outbound connection is deleted and cannot be used further.</li> </ul>\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrossClusterSearchConnectionStatusMessage\"\n        },\n        {\n          \"description\": \"Specifies verbose information for the outbound connection status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-outbound-cross-cluster-search-connection-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: OutboundCrossClusterSearchConnectionStatus
---
