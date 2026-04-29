---
description: ActivationResponse schema from Apache OpenWhisk
layout: schema
name: ActivationResponse
properties_list:
- description: Activation status
  name: status
  type: string
- description: HTTP status code equivalent
  name: statusCode
  type: integer
- description: ''
  name: success
  type: boolean
- description: Action result payload
  name: result
  type: object
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-activation-response-schema.json
slug: apache-openwhisk-activation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-response-schema.json\",\n  \"title\": \"ActivationResponse\",\n  \"description\": \"ActivationResponse schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Activation status\",\n      \"example\": \"success\",\n      \"enum\": [\n        \"success\",\n        \"application error\",\n        \"developer error\",\n        \"whisk internal error\"\n      ]\n    },\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code equivalent\",\n      \"example\": 0\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"Action result payload\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-response-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActivationResponse
---
