---
description: A widget in a CloudWatch dashboard.
layout: schema
name: DashboardWidget
properties_list:
- description: The type of the widget.
  name: type
  type: string
- description: The horizontal position of the widget on the dashboard grid.
  name: x
  type: integer
- description: The vertical position of the widget on the dashboard grid.
  name: y
  type: integer
- description: The width of the widget in grid units.
  name: width
  type: integer
- description: The height of the widget in grid units.
  name: height
  type: integer
- description: The properties for the widget, which vary depending on the widget type.
  name: properties
  type: object
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-dashboard-widget-schema.json
slug: cloudwatch-dashboard-widget
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardWidget\",\n  \"type\": \"object\",\n  \"description\": \"A widget in a CloudWatch dashboard.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the widget.\"\n    },\n    \"x\": {\n      \"type\": \"integer\",\n      \"description\": \"The horizontal position of the widget on the dashboard grid.\"\n    },\n    \"y\": {\n      \"type\": \"integer\",\n      \"description\": \"The vertical position of the widget on the dashboard grid.\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the widget in grid units.\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height of the widget in grid units.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties for the widget, which vary depending on the widget\
  \ type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-dashboard-widget-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DashboardWidget
---
