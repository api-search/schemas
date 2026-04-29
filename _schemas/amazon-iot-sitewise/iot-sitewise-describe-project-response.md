---
description: DescribeProjectResponse schema
layout: schema
name: DescribeProjectResponse
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: projectArn
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: portalId
  type: object
- description: ''
  name: projectDescription
  type: object
- description: ''
  name: projectCreationDate
  type: object
- description: ''
  name: projectLastUpdateDate
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-project-response-schema.json
slug: iot-sitewise-describe-project-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-project-response-schema.json\",\n  \"title\": \"DescribeProjectResponse\",\n  \"description\": \"DescribeProjectResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    },\n    \"projectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the project, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:project/${ProjectId}</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the project.\"\n        }\n      ]\n    },\n    \"portalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the portal that the project is in.\"\n        }\n      ]\n    },\n    \"projectDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The project's description.\"\n        }\n      ]\n    },\n    \"projectCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the project was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"projectLastUpdateDate\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the project was last updated, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectId\",\n    \"projectArn\",\n    \"projectName\",\n    \"portalId\",\n    \"projectCreationDate\",\n    \"projectLastUpdateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-project-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeProjectResponse
---
