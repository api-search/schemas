---
description: DescribeDashboardResponse schema
layout: schema
name: DescribeDashboardResponse
properties_list:
- description: ''
  name: dashboardId
  type: object
- description: ''
  name: dashboardArn
  type: object
- description: ''
  name: dashboardName
  type: object
- description: ''
  name: projectId
  type: object
- description: ''
  name: dashboardDescription
  type: object
- description: ''
  name: dashboardDefinition
  type: object
- description: ''
  name: dashboardCreationDate
  type: object
- description: ''
  name: dashboardLastUpdateDate
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-dashboard-response-schema.json
slug: iot-sitewise-describe-dashboard-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-dashboard-response-schema.json\",\n  \"title\": \"DescribeDashboardResponse\",\n  \"description\": \"DescribeDashboardResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dashboardId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the dashboard.\"\n        }\n      ]\n    },\n    \"dashboardArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the dashboard, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:dashboard/${DashboardId}</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"dashboardName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the dashboard.\"\n        }\n      ]\n    },\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the project that the dashboard is in.\"\n        }\n      ]\n    },\n    \"dashboardDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The dashboard's description.\"\n        }\n      ]\n    },\n    \"dashboardDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashboardDefinition\"\n        },\n        {\n          \"description\": \"The dashboard's definition JSON literal. For detailed information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/create-dashboards-using-aws-cli.html\\\
  \">Creating dashboards (CLI)</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    },\n    \"dashboardCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the dashboard was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"dashboardLastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the dashboard was last updated, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"dashboardId\",\n    \"dashboardArn\",\n    \"dashboardName\",\n    \"projectId\",\n    \"dashboardDefinition\",\n    \"dashboardCreationDate\",\n    \"dashboardLastUpdateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-dashboard-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeDashboardResponse
---
