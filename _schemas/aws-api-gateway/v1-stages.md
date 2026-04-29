---
description: Stages schema from Amazon API Gateway v1 API
layout: schema
name: Stages
properties_list:
- description: ''
  name: item
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-stages-schema.json
slug: v1-stages
source_filename: v1-stages-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"item\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"deploymentId\": {\n            \"type\": \"string\",\n            \"description\": \"Identifier of the deployment.\",\n            \"example\": \"abc123\"\n          },\n          \"stageName\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the stage.\",\n            \"example\": \"my-resource\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the stage.\",\n            \"example\": \"A description of this resource.\"\n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-stages-schema.json\"\
  ,\n  \"title\": \"Stages\",\n  \"description\": \"Stages schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-stages-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Stages
---
