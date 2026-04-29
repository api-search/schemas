---
description: ListDeploymentsResponse schema
layout: schema
name: ListDeploymentsResponse
properties_list:
- description: ''
  name: deployments
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-list-deployments-response-schema.json
slug: iot-greengrass-list-deployments-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-deployments-response-schema.json\",\n  \"title\": \"ListDeploymentsResponse\",\n  \"description\": \"ListDeploymentsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentList\"\n        },\n        {\n          \"description\": \"A list that summarizes each deployment.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextTokenString\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-deployments-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ListDeploymentsResponse
---
