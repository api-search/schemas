---
description: Performs an aggregation that will return a list of buckets. The list of buckets is a ranked list of the number of occurrences of an aggregation field value.
layout: schema
name: TermsAggregation
properties_list:
- description: ''
  name: maxBuckets
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-terms-aggregation-schema.json
slug: iot-core-terms-aggregation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-terms-aggregation-schema.json\",\n  \"title\": \"TermsAggregation\",\n  \"description\": \"Performs an aggregation that will return a list of buckets. The list of buckets is a ranked list of the number of occurrences of an aggregation field value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxBuckets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxBuckets\"\n        },\n        {\n          \"description\": \"The number of buckets to return in the response. Default to 10.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-terms-aggregation-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: TermsAggregation
---
