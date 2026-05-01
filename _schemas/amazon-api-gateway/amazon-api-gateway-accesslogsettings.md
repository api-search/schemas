---
description: ''
layout: schema
name: AccessLogSettings
properties_list:
- description: A single line format of the access logs of data using CLF, JSON, XML, or CSV format.
  name: format
  type: string
- description: The Amazon Resource Name (ARN) of the CloudWatch Logs log group or Kinesis Data Firehose delivery stream.
  name: destinationArn
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-accesslogsettings-schema.json
slug: amazon-api-gateway-accesslogsettings
source_filename: amazon-api-gateway-accesslogsettings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AccessLogSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"A single line format of the access logs of data using CLF, JSON, XML, or CSV format.\"\n    },\n    \"destinationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the CloudWatch Logs log group or Kinesis Data Firehose delivery stream.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-accesslogsettings-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: AccessLogSettings
---
