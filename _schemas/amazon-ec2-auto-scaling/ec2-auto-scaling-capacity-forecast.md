---
description: A <code>GetPredictiveScalingForecast</code> call returns the capacity forecast for a predictive scaling policy. This structure includes the data points for that capacity forecast, along with the timestamps of those data points.
layout: schema
name: CapacityForecast
properties_list:
- description: ''
  name: Timestamps
  type: object
- description: ''
  name: Values
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-capacity-forecast-schema.json
slug: ec2-auto-scaling-capacity-forecast
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-capacity-forecast-schema.json\",\n  \"title\": \"CapacityForecast\",\n  \"description\": \"A <code>GetPredictiveScalingForecast</code> call returns the capacity forecast for a predictive scaling policy. This structure includes the data points for that capacity forecast, along with the timestamps of those data points. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timestamps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingForecastTimestamps\"\n        },\n        {\n          \"description\": \"The timestamps for the data points, in UTC format.\"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredictiveScalingForecastValues\"\n        },\n       \
  \ {\n          \"description\": \"The values of the data points.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Timestamps\",\n    \"Values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-capacity-forecast-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: CapacityForecast
---
