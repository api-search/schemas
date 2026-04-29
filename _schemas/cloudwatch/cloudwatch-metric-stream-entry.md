---
description: Contains information about a metric stream.
layout: schema
name: MetricStreamEntry
properties_list:
- description: The ARN of the metric stream.
  name: Arn
  type: string
- description: The date when the metric stream was created.
  name: CreationDate
  type: string
- description: The date when the metric stream was last updated.
  name: LastUpdateDate
  type: string
- description: The name of the metric stream.
  name: Name
  type: string
- description: The ARN of the Kinesis Data Firehose delivery stream used by this metric stream.
  name: FirehoseArn
  type: string
- description: The current state of the metric stream.
  name: State
  type: string
- description: The output format of the metric stream.
  name: OutputFormat
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-stream-entry-schema.json
slug: cloudwatch-metric-stream-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricStreamEntry\",\n  \"type\": \"object\",\n  \"description\": \"Contains information about a metric stream.\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the metric stream.\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date when the metric stream was created.\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date when the metric stream was last updated.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric stream.\"\n    },\n    \"FirehoseArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Kinesis Data Firehose delivery stream used by this metric stream.\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the\
  \ metric stream.\"\n    },\n    \"OutputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The output format of the metric stream.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-stream-entry-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricStreamEntry
---
