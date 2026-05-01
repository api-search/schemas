---
description: Contains information about a composite model property on an asset.
layout: schema
name: CompositeModelProperty
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: Contains asset property information.
  name: assetProperty
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-composite-model-property-schema.json
slug: iot-sitewise-composite-model-property
source_filename: iot-sitewise-composite-model-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-composite-model-property-schema.json\",\n  \"title\": \"CompositeModelProperty\",\n  \"description\": \"Contains information about a composite model property on an asset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the property.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The type of the composite model that defines this property.\"\n        }\n      ]\n    },\n    \"assetProperty\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"\
  dataType\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ID\"\n            },\n            {\n              \"description\": \"The ID of the asset property.\"\n            }\n          ]\n        },\n        \"name\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Name\"\n            },\n            {\n              \"description\": \"The name of the property.\"\n            }\n          ]\n        },\n        \"alias\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyAlias\"\n            },\n            {\n              \"description\": \"The alias that identifies the property, such as an OPC-UA server data stream path (for example, <code>/company/windfarm/3/turbine/7/temperature</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/connect-data-streams.html\\\
  \">Mapping industrial data streams to asset properties</a> in the <i>IoT SiteWise User Guide</i>.\"\n            }\n          ]\n        },\n        \"notification\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyNotification\"\n            },\n            {\n              \"description\": \"The asset property's notification topic and state. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_UpdateAssetProperty.html\\\">UpdateAssetProperty</a>.\"\n            }\n          ]\n        },\n        \"dataType\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyDataType\"\n            },\n            {\n              \"description\": \"The property data type.\"\n            }\n          ]\n        },\n        \"unit\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyUnit\"\n            },\n   \
  \         {\n              \"description\": \"The unit (such as <code>Newtons</code> or <code>RPM</code>) of the asset property.\"\n            }\n          ]\n        },\n        \"type\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/PropertyType\"\n            },\n            {\n              \"description\": \"The property type (see <code>PropertyType</code>). A property contains one type.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Contains asset property information.\"\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \" The ID of the composite model that contains the property. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"assetProperty\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-composite-model-property-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CompositeModelProperty
---
