---
description: GetPredictiveScalingForecastAnswer schema from Auto Scaling
layout: schema
name: GetPredictiveScalingForecastAnswer
properties_list:
- description: ''
  name: LoadForecast
  type: object
- description: ''
  name: CapacityForecast
  type: object
- description: ''
  name: UpdateTime
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-get-predictive-scaling-forecast-answer-schema.json
slug: ec2-auto-scaling-get-predictive-scaling-forecast-answer
source_filename: ec2-auto-scaling-get-predictive-scaling-forecast-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-get-predictive-scaling-forecast-answer-schema.json\",\n  \"title\": \"GetPredictiveScalingForecastAnswer\",\n  \"description\": \"GetPredictiveScalingForecastAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoadForecast\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadForecasts\"\n        },\n        {\n          \"description\": \"The load forecast.\"\n        }\n      ]\n    },\n    \"CapacityForecast\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityForecast\"\n        },\n        {\n          \"description\": \"The capacity forecast.\"\n        }\n      ]\n    },\n    \"UpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\
  \n        },\n        {\n          \"description\": \"The time the forecast was made.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LoadForecast\",\n    \"CapacityForecast\",\n    \"UpdateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-get-predictive-scaling-forecast-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: GetPredictiveScalingForecastAnswer
---
