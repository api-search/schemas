---
description: DescribeGatewayCapabilityConfigurationResponse schema
layout: schema
name: DescribeGatewayCapabilityConfigurationResponse
properties_list:
- description: ''
  name: gatewayId
  type: object
- description: ''
  name: capabilityNamespace
  type: object
- description: ''
  name: capabilityConfiguration
  type: object
- description: ''
  name: capabilitySyncStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-gateway-capability-configuration-response-schema.json
slug: iot-sitewise-describe-gateway-capability-configuration-response
source_filename: iot-sitewise-describe-gateway-capability-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-gateway-capability-configuration-response-schema.json\",\n  \"title\": \"DescribeGatewayCapabilityConfigurationResponse\",\n  \"description\": \"DescribeGatewayCapabilityConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewayId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the gateway that defines the capability configuration.\"\n        }\n      ]\n    },\n    \"capabilityNamespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilityNamespace\"\n        },\n        {\n          \"description\": \"The namespace of the gateway capability.\"\n        }\n      ]\n    },\n    \"capabilityConfiguration\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilityConfiguration\"\n        },\n        {\n          \"description\": \"The JSON document that defines the gateway capability's configuration. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/configure-sources.html#configure-source-cli\\\">Configuring data sources (CLI)</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    },\n    \"capabilitySyncStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilitySyncStatus\"\n        },\n        {\n          \"description\": \"<p>The synchronization status of the capability configuration. The sync status can be one of the following:</p> <ul> <li> <p> <code>IN_SYNC</code> \\u2013 The gateway is running the capability configuration.</p> </li> <li> <p> <code>OUT_OF_SYNC</code> \\u2013 The gateway hasn't received the capability configuration.</p> </li> <li> <p> <code>SYNC_FAILED</code>\
  \ \\u2013 The gateway rejected the capability configuration.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewayId\",\n    \"capabilityNamespace\",\n    \"capabilityConfiguration\",\n    \"capabilitySyncStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-gateway-capability-configuration-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeGatewayCapabilityConfigurationResponse
---
