---
description: GetSampleDataRequest schema from Amazon Lookout for Metrics API
layout: schema
name: GetSampleDataRequest
properties_list:
- description: ''
  name: S3SourceConfig
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-sample-data-request-schema.json
slug: amazon-lookout-for-metrics-get-sample-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-sample-data-request-schema.json\",\n  \"title\": \"GetSampleDataRequest\",\n  \"description\": \"GetSampleDataRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3SourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleDataS3SourceConfig\"\n        },\n        {\n          \"description\": \"A datasource bucket in Amazon S3.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-sample-data-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetSampleDataRequest
---
