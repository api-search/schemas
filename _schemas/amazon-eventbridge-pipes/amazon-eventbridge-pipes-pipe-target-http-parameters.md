---
description: These are custom parameter to be used when the target is an API Gateway REST APIs or EventBridge ApiDestinations.
layout: schema
name: PipeTargetHttpParameters
properties_list:
- description: ''
  name: HeaderParameters
  type: object
- description: ''
  name: PathParameterValues
  type: object
- description: ''
  name: QueryStringParameters
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-http-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-http-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-http-parameters-schema.json\",\n  \"title\": \"PipeTargetHttpParameters\",\n  \"description\": \"These are custom parameter to be used when the target is an API Gateway REST APIs or EventBridge ApiDestinations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HeaderParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderParametersMap\"\n        },\n        {\n          \"description\": \"The headers that need to be sent as part of request invoking the API Gateway REST API or EventBridge ApiDestination.\"\n        }\n      ]\n    },\n    \"PathParameterValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathParameterList\"\n        },\n        {\n          \"description\": \"\
  The path parameter values to be used to populate API Gateway REST API or EventBridge ApiDestination path wildcards (\\\"*\\\").\"\n        }\n      ]\n    },\n    \"QueryStringParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryStringParametersMap\"\n        },\n        {\n          \"description\": \"The query string keys/values that need to be sent as part of request invoking the API Gateway REST API or EventBridge ApiDestination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-http-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetHttpParameters
---
