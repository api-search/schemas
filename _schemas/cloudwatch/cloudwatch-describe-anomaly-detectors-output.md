---
description: ''
layout: schema
name: DescribeAnomalyDetectorsOutput
properties_list:
- description: The list of anomaly detection models returned by the operation.
  name: AnomalyDetectors
  type: array
- description: A token that you can use in a subsequent operation to retrieve the next set of results.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-anomaly-detectors-output-schema.json
slug: cloudwatch-describe-anomaly-detectors-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAnomalyDetectorsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectors\": {\n      \"type\": \"array\",\n      \"description\": \"The list of anomaly detection models returned by the operation.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"A token that you can use in a subsequent operation to retrieve the next set of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-anomaly-detectors-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAnomalyDetectorsOutput
---
