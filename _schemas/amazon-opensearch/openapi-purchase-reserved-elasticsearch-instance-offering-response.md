---
description: Represents the output of a <code>PurchaseReservedElasticsearchInstanceOffering</code> operation.
layout: schema
name: PurchaseReservedElasticsearchInstanceOfferingResponse
properties_list:
- description: ''
  name: ReservedElasticsearchInstanceId
  type: object
- description: ''
  name: ReservationName
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-purchase-reserved-elasticsearch-instance-offering-response-schema.json
slug: openapi-purchase-reserved-elasticsearch-instance-offering-response
source_filename: openapi-purchase-reserved-elasticsearch-instance-offering-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-purchase-reserved-elasticsearch-instance-offering-response-schema.json\",\n  \"title\": \"PurchaseReservedElasticsearchInstanceOfferingResponse\",\n  \"description\": \"Represents the output of a <code>PurchaseReservedElasticsearchInstanceOffering</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedElasticsearchInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GUID\"\n        },\n        {\n          \"description\": \"Details of the reserved Elasticsearch instance which was purchased.\"\n        }\n      ]\n    },\n    \"ReservationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationToken\"\n        },\n        {\n          \"description\": \"The customer-specified identifier used\
  \ to track this reservation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-purchase-reserved-elasticsearch-instance-offering-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: PurchaseReservedElasticsearchInstanceOfferingResponse
---
