---
description: ''
layout: schema
name: DescribeAnomalyDetectorsInput
properties_list:
- description: Use the token returned by the previous operation to request the next page of results.
  name: NextToken
  type: string
- description: The maximum number of results to return in one operation.
  name: MaxResults
  type: integer
- description: Limits the results to only the anomaly detection models that are associated with the specified namespace.
  name: Namespace
  type: string
- description: Limits the results to only the anomaly detection models that are associated with the specified metric name.
  name: MetricName
  type: string
- description: Limits the results to only the anomaly detection models that are associated with the specified metric dimensions.
  name: Dimensions
  type: array
- description: The anomaly detector types to request when using DescribeAnomalyDetectors.
  name: AnomalyDetectorTypes
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-anomaly-detectors-input-schema.json
slug: cloudwatch-describe-anomaly-detectors-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAnomalyDetectorsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Use the token returned by the previous operation to request the next page of results.\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to return in one operation.\"\n    },\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Limits the results to only the anomaly detection models that are associated with the specified namespace.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"Limits the results to only the anomaly detection models that are associated with the specified metric name.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"Limits the results to only the anomaly\
  \ detection models that are associated with the specified metric dimensions.\"\n    },\n    \"AnomalyDetectorTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The anomaly detector types to request when using DescribeAnomalyDetectors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-anomaly-detectors-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAnomalyDetectorsInput
---
