---
description: Contains the specific price and frequency of a recurring charges for a reserved Elasticsearch instance, or for a reserved Elasticsearch instance offering.
layout: schema
name: RecurringCharge
properties_list:
- description: ''
  name: RecurringChargeAmount
  type: object
- description: ''
  name: RecurringChargeFrequency
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-recurring-charge-schema.json
slug: openapi-recurring-charge
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-recurring-charge-schema.json\",\n  \"title\": \"RecurringCharge\",\n  \"description\": \"Contains the specific price and frequency of a recurring charges for a reserved Elasticsearch instance, or for a reserved Elasticsearch instance offering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecurringChargeAmount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The monetary amount of the recurring charge.\"\n        }\n      ]\n    },\n    \"RecurringChargeFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The frequency of the recurring charge.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-recurring-charge-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: RecurringCharge
---
