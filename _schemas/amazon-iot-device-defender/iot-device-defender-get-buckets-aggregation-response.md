---
description: GetBucketsAggregationResponse schema
layout: schema
name: GetBucketsAggregationResponse
properties_list:
- description: ''
  name: totalCount
  type: object
- description: ''
  name: buckets
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-get-buckets-aggregation-response-schema.json
slug: iot-device-defender-get-buckets-aggregation-response
source_filename: iot-device-defender-get-buckets-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-buckets-aggregation-response-schema.json\",\n  \"title\": \"GetBucketsAggregationResponse\",\n  \"description\": \"GetBucketsAggregationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Count\"\n        },\n        {\n          \"description\": \"The total number of things that fit the query string criteria.\"\n        }\n      ]\n    },\n    \"buckets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Buckets\"\n        },\n        {\n          \"description\": \"<p>The main part of the response with a list of buckets. Each bucket contains a <code>keyValue</code> and a <code>count</code>.</p> <p> <code>keyValue</code>: The aggregation\
  \ field value counted for the particular bucket.</p> <p> <code>count</code>: The number of documents that have that value.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-buckets-aggregation-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: GetBucketsAggregationResponse
---
