---
description: GetSampleDataResponse schema from Amazon Lookout for Metrics API
layout: schema
name: GetSampleDataResponse
properties_list:
- description: ''
  name: HeaderValues
  type: object
- description: ''
  name: SampleRows
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-sample-data-response-schema.json
slug: amazon-lookout-for-metrics-get-sample-data-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-sample-data-response-schema.json\",\n  \"title\": \"GetSampleDataResponse\",\n  \"description\": \"GetSampleDataResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HeaderValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderValueList\"\n        },\n        {\n          \"description\": \"A list of header labels for the records.\"\n        }\n      ]\n    },\n    \"SampleRows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleRows\"\n        },\n        {\n          \"description\": \"A list of records.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-sample-data-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetSampleDataResponse
---
