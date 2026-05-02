---
description: A cost forecast projecting future Kubernetes workload spend based on historical allocation data and trends.
layout: schema
name: Kubecost Forecast
properties_list:
- description: Total forecasted cost for the forecast window.
  name: totalCost
  type: number
- description: Confidence level of the forecast (0-1).
  name: confidence
  type: number
- description: The time window for the forecast projection.
  name: forecastWindow
  type: object
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/forecast.json
slug: forecast
source_filename: forecast.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/forecast.json\",\n  \"title\": \"Kubecost Forecast\",\n  \"description\": \"A cost forecast projecting future Kubernetes workload spend based on historical allocation data and trends.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total forecasted cost for the forecast window.\"\n    },\n    \"confidence\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence level of the forecast (0-1).\"\n    },\n    \"forecastWindow\": {\n      \"type\": \"object\",\n      \"description\": \"The time window for the forecast projection.\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Start of the forecast window.\"\n        },\n        \"end\": {\n  \
  \        \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"End of the forecast window.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/forecast.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Forecast
---
