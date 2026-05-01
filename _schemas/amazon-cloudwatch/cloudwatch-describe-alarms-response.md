---
description: Response from the DescribeAlarms action
layout: schema
name: DescribeAlarmsResponse
properties_list:
- description: The information about the alarms
  name: metricAlarms
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-describe-alarms-response-schema.json
slug: cloudwatch-describe-alarms-response
source_filename: cloudwatch-describe-alarms-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarms-response-schema.json\",\n  \"title\": \"DescribeAlarmsResponse\",\n  \"description\": \"Response from the DescribeAlarms action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricAlarms\": {\n      \"type\": \"array\",\n      \"description\": \"The information about the alarms\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Alarm\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarms-response-schema.json
tags:
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: DescribeAlarmsResponse
---
