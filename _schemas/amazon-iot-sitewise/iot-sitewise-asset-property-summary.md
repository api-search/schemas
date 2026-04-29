---
description: Contains a summary of a property associated with an asset.
layout: schema
name: AssetPropertySummary
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: alias
  type: object
- description: ''
  name: unit
  type: object
- description: Contains asset property value notification information. When the notification state is enabled, IoT SiteWise publishes property value updates to a unique MQTT topic. For more information, see <a href=
  name: notification
  type: object
- description: ''
  name: assetCompositeModelId
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-property-summary-schema.json
slug: iot-sitewise-asset-property-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-summary-schema.json\",\n  \"title\": \"AssetPropertySummary\",\n  \"description\": \"Contains a summary of a property associated with an asset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the property.\"\n        }\n      ]\n    },\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyAlias\"\n        },\n        {\n          \"description\": \"The alias that identifies the property, such as an OPC-UA server data stream path (for example, <code>/company/windfarm/3/turbine/7/temperature</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/connect-data-streams.html\\\
  \">Mapping industrial data streams to asset properties</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyUnit\"\n        },\n        {\n          \"description\": \" The unit of measure (such as Newtons or RPM) of the asset property. \"\n        }\n      ]\n    },\n    \"notification\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"topic\",\n        \"state\"\n      ],\n      \"properties\": {\n        \"topic\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyNotificationTopic\"\n            },\n            {\n              \"description\": \"The MQTT topic to which IoT SiteWise publishes property value update notifications.\"\n            }\n          ]\n        },\n        \"state\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyNotificationState\"\
  \n            },\n            {\n              \"description\": \"The current notification state.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Contains asset property value notification information. When the notification state is enabled, IoT SiteWise publishes property value updates to a unique MQTT topic. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/interact-with-other-services.html\\\">Interacting with other services</a> in the <i>IoT SiteWise User Guide</i>.\"\n    },\n    \"assetCompositeModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \" The ID of the composite model that contains the asset property. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-summary-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetPropertySummary
---
