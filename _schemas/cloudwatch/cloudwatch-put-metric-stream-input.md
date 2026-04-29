---
description: ''
layout: schema
name: PutMetricStreamInput
properties_list:
- description: The name of the metric stream.
  name: Name
  type: string
- description: If you specify this parameter, the stream sends only the metrics from the metric namespaces that you specify here.
  name: IncludeFilters
  type: array
- description: If you specify this parameter, the stream sends metrics from all metric namespaces except for the namespaces that you specify here.
  name: ExcludeFilters
  type: array
- description: The ARN of the Amazon Kinesis Data Firehose delivery stream to use for this metric stream.
  name: FirehoseArn
  type: string
- description: The ARN of an IAM role that this metric stream will use to access Amazon Kinesis Data Firehose resources.
  name: RoleArn
  type: string
- description: The output format for the stream.
  name: OutputFormat
  type: string
- description: A list of key-value pairs to associate with the metric stream.
  name: Tags
  type: array
- description: If you are creating a metric stream in a monitoring account, specify true to include metrics from source accounts.
  name: IncludeLinkedAccountsMetrics
  type: boolean
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-metric-stream-input-schema.json
slug: cloudwatch-put-metric-stream-input
source_filename: cloudwatch-put-metric-stream-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutMetricStreamInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric stream.\"\n    },\n    \"IncludeFilters\": {\n      \"type\": \"array\",\n      \"description\": \"If you specify this parameter, the stream sends only the metrics from the metric namespaces that you specify here.\"\n    },\n    \"ExcludeFilters\": {\n      \"type\": \"array\",\n      \"description\": \"If you specify this parameter, the stream sends metrics from all metric namespaces except for the namespaces that you specify here.\"\n    },\n    \"FirehoseArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Amazon Kinesis Data Firehose delivery stream to use for this metric stream.\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of an IAM role that this metric\
  \ stream will use to access Amazon Kinesis Data Firehose resources.\"\n    },\n    \"OutputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The output format for the stream.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of key-value pairs to associate with the metric stream.\"\n    },\n    \"IncludeLinkedAccountsMetrics\": {\n      \"type\": \"boolean\",\n      \"description\": \"If you are creating a metric stream in a monitoring account, specify true to include metrics from source accounts.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-metric-stream-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutMetricStreamInput
---
