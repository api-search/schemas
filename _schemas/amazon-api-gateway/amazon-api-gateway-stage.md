---
description: ''
layout: schema
name: Stage
properties_list:
- description: The identifier of the deployment attached to this stage.
  name: deploymentId
  type: string
- description: The identifier of a client certificate for an API stage.
  name: clientCertificateId
  type: string
- description: The name of the stage.
  name: stageName
  type: string
- description: The stage's description.
  name: description
  type: string
- description: Whether cache clustering is enabled for the stage.
  name: cacheClusterEnabled
  type: boolean
- description: The stage's cache cluster size.
  name: cacheClusterSize
  type: string
- description: ''
  name: cacheClusterStatus
  type: string
- description: ''
  name: methodSettings
  type: object
- description: Stage variables.
  name: variables
  type: object
- description: ''
  name: documentationVersion
  type: string
- description: ''
  name: accessLogSettings
  type: object
- description: ''
  name: canarySettings
  type: object
- description: Whether X-Ray tracing is enabled for this stage.
  name: tracingEnabled
  type: boolean
- description: The ARN of the WebAcl associated with the stage.
  name: webAclArn
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: createdDate
  type: string
- description: ''
  name: lastUpdatedDate
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-stage-schema.json
slug: amazon-api-gateway-stage
source_filename: amazon-api-gateway-stage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Stage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the deployment attached to this stage.\"\n    },\n    \"clientCertificateId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of a client certificate for an API stage.\"\n    },\n    \"stageName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stage.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The stage's description.\"\n    },\n    \"cacheClusterEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether cache clustering is enabled for the stage.\"\n    },\n    \"cacheClusterSize\": {\n      \"type\": \"string\",\n      \"description\": \"The stage's cache cluster size.\",\n      \"enum\": [\n        \"0.5\",\n        \"1.6\",\n    \
  \    \"6.1\",\n        \"13.5\",\n        \"28.4\",\n        \"58.2\",\n        \"118\",\n        \"237\"\n      ]\n    },\n    \"cacheClusterStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_IN_PROGRESS\",\n        \"AVAILABLE\",\n        \"DELETE_IN_PROGRESS\",\n        \"NOT_AVAILABLE\",\n        \"FLUSH_IN_PROGRESS\"\n      ]\n    },\n    \"methodSettings\": {\n      \"type\": \"object\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Stage variables.\"\n    },\n    \"documentationVersion\": {\n      \"type\": \"string\"\n    },\n    \"accessLogSettings\": {\n      \"$ref\": \"#/definitions/AccessLogSettings\"\n    },\n    \"canarySettings\": {\n      \"$ref\": \"#/definitions/CanarySettings\"\n    },\n    \"tracingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether X-Ray tracing is enabled for this stage.\"\n    },\n    \"webAclArn\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The ARN of the WebAcl associated with the stage.\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-stage-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Stage
---
