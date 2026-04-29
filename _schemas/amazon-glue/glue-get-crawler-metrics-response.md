---
description: GetCrawlerMetricsResponse schema from Amazon Glue API
layout: schema
name: GetCrawlerMetricsResponse
properties_list:
- description: ''
  name: CrawlerMetricsList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-crawler-metrics-response-schema.json
slug: glue-get-crawler-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-crawler-metrics-response-schema.json\",\n  \"title\": \"GetCrawlerMetricsResponse\",\n  \"description\": \"GetCrawlerMetricsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrawlerMetricsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrawlerMetricsList\"\n        },\n        {\n          \"description\": \"A list of metrics for the specified crawler.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list does not contain the last metric available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-crawler-metrics-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetCrawlerMetricsResponse
---
