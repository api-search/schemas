---
description: DescribeAnomalyDetectionExecutionsResponse schema from Amazon Lookout for Metrics API
layout: schema
name: DescribeAnomalyDetectionExecutionsResponse
properties_list:
- description: ''
  name: ExecutionList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-describe-anomaly-detection-executions-response-schema.json
slug: amazon-lookout-for-metrics-describe-anomaly-detection-executions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-anomaly-detection-executions-response-schema.json\",\n  \"title\": \"DescribeAnomalyDetectionExecutionsResponse\",\n  \"description\": \"DescribeAnomalyDetectionExecutionsResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExecutionList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionList\"\n        },\n        {\n          \"description\": \"A list of detection jobs.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token that's included if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-anomaly-detection-executions-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DescribeAnomalyDetectionExecutionsResponse
---
