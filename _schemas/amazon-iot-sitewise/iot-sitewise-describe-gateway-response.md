---
description: DescribeGatewayResponse schema
layout: schema
name: DescribeGatewayResponse
properties_list:
- description: ''
  name: gatewayId
  type: object
- description: ''
  name: gatewayName
  type: object
- description: ''
  name: gatewayArn
  type: object
- description: ''
  name: gatewayPlatform
  type: object
- description: ''
  name: gatewayCapabilitySummaries
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastUpdateDate
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-gateway-response-schema.json
slug: iot-sitewise-describe-gateway-response
source_filename: iot-sitewise-describe-gateway-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-gateway-response-schema.json\",\n  \"title\": \"DescribeGatewayResponse\",\n  \"description\": \"DescribeGatewayResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the gateway device.\"\n        }\n      ]\n    },\n    \"gatewayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the gateway.\"\n        }\n      ]\n    },\n    \"gatewayArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\
  \">ARN</a> of the gateway, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:gateway/${GatewayId}</code> </p>\"\n        }\n      ]\n    },\n    \"gatewayPlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayPlatform\"\n        },\n        {\n          \"description\": \"The gateway's platform.\"\n        }\n      ]\n    },\n    \"gatewayCapabilitySummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayCapabilitySummaries\"\n        },\n        {\n          \"description\": \"A list of gateway capability summaries that each contain a namespace and status. Each gateway capability defines data sources for the gateway. To retrieve a capability configuration's definition, use <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_DescribeGatewayCapabilityConfiguration.html\\\">DescribeGatewayCapabilityConfiguration</a>.\"\n        }\n      ]\n\
  \    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the gateway was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"lastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the gateway was last updated, in Unix epoch time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewayId\",\n    \"gatewayName\",\n    \"gatewayArn\",\n    \"gatewayCapabilitySummaries\",\n    \"creationDate\",\n    \"lastUpdateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-gateway-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeGatewayResponse
---
