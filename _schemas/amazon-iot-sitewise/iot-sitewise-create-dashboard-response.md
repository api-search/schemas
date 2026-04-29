---
description: CreateDashboardResponse schema
layout: schema
name: CreateDashboardResponse
properties_list:
- description: ''
  name: dashboardId
  type: object
- description: ''
  name: dashboardArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-dashboard-response-schema.json
slug: iot-sitewise-create-dashboard-response
source_filename: iot-sitewise-create-dashboard-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-dashboard-response-schema.json\",\n  \"title\": \"CreateDashboardResponse\",\n  \"description\": \"CreateDashboardResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dashboardId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the dashboard.\"\n        }\n      ]\n    },\n    \"dashboardArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the dashboard, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:dashboard/${DashboardId}</code>\
  \ </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dashboardId\",\n    \"dashboardArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-dashboard-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreateDashboardResponse
---
