---
description: Contains an asset model property definition. This property definition is applied to all assets created from the asset model.
layout: schema
name: AssetModelPropertyDefinition
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: dataType
  type: object
- description: ''
  name: dataTypeSpec
  type: object
- description: ''
  name: unit
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-model-property-definition-schema.json
slug: iot-sitewise-asset-model-property-definition
source_filename: iot-sitewise-asset-model-property-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-property-definition-schema.json\",\n  \"title\": \"AssetModelPropertyDefinition\",\n  \"description\": \"Contains an asset model property definition. This property definition is applied to all assets created from the asset model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the property definition.\"\n        }\n      ]\n    },\n    \"dataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyDataType\"\n        },\n        {\n          \"description\": \"<p>The data type of the property definition.</p> <p>If you specify <code>STRUCT</code>, you must also specify <code>dataTypeSpec</code>\
  \ to identify the type of the structure for this property.</p>\"\n        }\n      ]\n    },\n    \"dataTypeSpec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The data type of the structure for this property. This parameter is required on properties that have the <code>STRUCT</code> data type.</p> <p>The options for this parameter depend on the type of the composite model in which you define this property. Use <code>AWS/ALARM_STATE</code> for alarm state in alarm composite models.</p>\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyUnit\"\n        },\n        {\n          \"description\": \"The unit of the property definition, such as <code>Newtons</code> or <code>RPM</code>.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyType\"\
  \n        },\n        {\n          \"description\": \"The property definition type (see <code>PropertyType</code>). You can only specify one type in a property definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"dataType\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-model-property-definition-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetModelPropertyDefinition
---
