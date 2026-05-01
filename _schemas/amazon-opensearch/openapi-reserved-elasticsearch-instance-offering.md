---
description: Details of a reserved Elasticsearch instance offering.
layout: schema
name: ReservedElasticsearchInstanceOffering
properties_list:
- description: ''
  name: ReservedElasticsearchInstanceOfferingId
  type: object
- description: ''
  name: ElasticsearchInstanceType
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: FixedPrice
  type: object
- description: ''
  name: UsagePrice
  type: object
- description: ''
  name: CurrencyCode
  type: object
- description: ''
  name: PaymentOption
  type: object
- description: ''
  name: RecurringCharges
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-reserved-elasticsearch-instance-offering-schema.json
slug: openapi-reserved-elasticsearch-instance-offering
source_filename: openapi-reserved-elasticsearch-instance-offering-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-reserved-elasticsearch-instance-offering-schema.json\",\n  \"title\": \"ReservedElasticsearchInstanceOffering\",\n  \"description\": \"Details of a reserved Elasticsearch instance offering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedElasticsearchInstanceOfferingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GUID\"\n        },\n        {\n          \"description\": \"The Elasticsearch reserved instance offering identifier.\"\n        }\n      ]\n    },\n    \"ElasticsearchInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ESPartitionInstanceType\"\n        },\n        {\n          \"description\": \"The Elasticsearch instance type offered by the reserved instance offering.\"\n        }\n      ]\n\
  \    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The duration, in seconds, for which the offering will reserve the Elasticsearch instance.\"\n        }\n      ]\n    },\n    \"FixedPrice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The upfront fixed charge you will pay to purchase the specific reserved Elasticsearch instance offering. \"\n        }\n      ]\n    },\n    \"UsagePrice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The rate you are charged for each hour the domain that is using the offering is running.\"\n        }\n      ]\n    },\n    \"CurrencyCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n    \
  \      \"description\": \"The currency code for the reserved Elasticsearch instance offering.\"\n        }\n      ]\n    },\n    \"PaymentOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservedElasticsearchInstancePaymentOption\"\n        },\n        {\n          \"description\": \"Payment option for the reserved Elasticsearch instance offering\"\n        }\n      ]\n    },\n    \"RecurringCharges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecurringChargeList\"\n        },\n        {\n          \"description\": \"The charge to your account regardless of whether you are creating any domains using the instance offering.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-reserved-elasticsearch-instance-offering-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ReservedElasticsearchInstanceOffering
---
