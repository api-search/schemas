---
description: ''
layout: schema
name: DescribeAlarmHistoryOutput
properties_list:
- description: The alarm histories, in JSON format.
  name: AlarmHistoryItems
  type: array
- description: The token that marks the start of the next batch of returned results.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-alarm-history-output-schema.json
slug: cloudwatch-describe-alarm-history-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAlarmHistoryOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmHistoryItems\": {\n      \"type\": \"array\",\n      \"description\": \"The alarm histories, in JSON format.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token that marks the start of the next batch of returned results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarm-history-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAlarmHistoryOutput
---
