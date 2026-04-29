---
description: ''
layout: schema
name: DescribeAlarmsOutput
properties_list:
- description: The information about any metric alarms returned by the operation.
  name: MetricAlarms
  type: array
- description: The information about any composite alarms returned by the operation.
  name: CompositeAlarms
  type: array
- description: The token that marks the start of the next batch of returned results.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-alarms-output-schema.json
slug: cloudwatch-describe-alarms-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAlarmsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricAlarms\": {\n      \"type\": \"array\",\n      \"description\": \"The information about any metric alarms returned by the operation.\"\n    },\n    \"CompositeAlarms\": {\n      \"type\": \"array\",\n      \"description\": \"The information about any composite alarms returned by the operation.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token that marks the start of the next batch of returned results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarms-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAlarmsOutput
---
