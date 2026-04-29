---
description: Represents a set of statistics that describes a specific metric.
layout: schema
name: StatisticSet
properties_list:
- description: The number of samples used for the statistic set.
  name: SampleCount
  type: number
- description: The sum of values for the sample set.
  name: Sum
  type: number
- description: The minimum value of the sample set.
  name: Minimum
  type: number
- description: The maximum value of the sample set.
  name: Maximum
  type: number
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-statistic-set-schema.json
slug: cloudwatch-statistic-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatisticSet\",\n  \"type\": \"object\",\n  \"description\": \"Represents a set of statistics that describes a specific metric.\",\n  \"properties\": {\n    \"SampleCount\": {\n      \"type\": \"number\",\n      \"description\": \"The number of samples used for the statistic set.\"\n    },\n    \"Sum\": {\n      \"type\": \"number\",\n      \"description\": \"The sum of values for the sample set.\"\n    },\n    \"Minimum\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum value of the sample set.\"\n    },\n    \"Maximum\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum value of the sample set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-statistic-set-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: StatisticSet
---
