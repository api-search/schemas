---
description: Performs an aggregation that will return a list of buckets. The list of buckets is a ranked list of the number of occurrences of an aggregation field value.
layout: schema
name: TermsAggregation
properties_list:
- description: ''
  name: maxBuckets
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-terms-aggregation-schema.json
slug: iot-device-defender-terms-aggregation
source_filename: iot-device-defender-terms-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-terms-aggregation-schema.json\",\n  \"title\": \"TermsAggregation\",\n  \"description\": \"Performs an aggregation that will return a list of buckets. The list of buckets is a ranked list of the number of occurrences of an aggregation field value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxBuckets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxBuckets\"\n        },\n        {\n          \"description\": \"The number of buckets to return in the response. Default to 10.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-terms-aggregation-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: TermsAggregation
---
