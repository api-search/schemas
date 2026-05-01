---
description: Container for parameters to <code>PurchaseReservedElasticsearchInstanceOffering</code>
layout: schema
name: PurchaseReservedElasticsearchInstanceOfferingRequest
properties_list:
- description: ''
  name: ReservedElasticsearchInstanceOfferingId
  type: object
- description: ''
  name: ReservationName
  type: object
- description: ''
  name: InstanceCount
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-purchase-reserved-elasticsearch-instance-offering-request-schema.json
slug: openapi-purchase-reserved-elasticsearch-instance-offering-request
source_filename: openapi-purchase-reserved-elasticsearch-instance-offering-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-purchase-reserved-elasticsearch-instance-offering-request-schema.json\",\n  \"title\": \"PurchaseReservedElasticsearchInstanceOfferingRequest\",\n  \"description\": \"Container for parameters to <code>PurchaseReservedElasticsearchInstanceOffering</code>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedElasticsearchInstanceOfferingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GUID\"\n        },\n        {\n          \"description\": \"The ID of the reserved Elasticsearch instance offering to purchase.\"\n        }\n      ]\n    },\n    \"ReservationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationToken\"\n        },\n        {\n          \"description\": \"A customer-specified identifier to track\
  \ this reservation.\"\n        }\n      ]\n    },\n    \"InstanceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceCount\"\n        },\n        {\n          \"description\": \"The number of Elasticsearch instances to reserve.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ReservedElasticsearchInstanceOfferingId\",\n    \"ReservationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-purchase-reserved-elasticsearch-instance-offering-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: PurchaseReservedElasticsearchInstanceOfferingRequest
---
