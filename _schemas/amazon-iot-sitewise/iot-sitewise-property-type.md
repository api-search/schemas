---
description: Contains a property type, which can be one of <code>attribute</code>, <code>measurement</code>, <code>metric</code>, or <code>transform</code>.
layout: schema
name: PropertyType
properties_list:
- description: ''
  name: attribute
  type: object
- description: ''
  name: measurement
  type: object
- description: ''
  name: transform
  type: object
- description: ''
  name: metric
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-property-type-schema.json
slug: iot-sitewise-property-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-property-type-schema.json\",\n  \"title\": \"PropertyType\",\n  \"description\": \"Contains a property type, which can be one of <code>attribute</code>, <code>measurement</code>, <code>metric</code>, or <code>transform</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attribute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attribute\"\n        },\n        {\n          \"description\": \"Specifies an asset attribute property. An attribute generally contains static information, such as the serial number of an <a href=\\\"https://en.wikipedia.org/wiki/Internet_of_things#Industrial_applications\\\">IIoT</a> wind turbine.\"\n        }\n      ]\n    },\n    \"measurement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Measurement\"\
  \n        },\n        {\n          \"description\": \"Specifies an asset measurement property. A measurement represents a device's raw sensor data stream, such as timestamped temperature values or timestamped power values.\"\n        }\n      ]\n    },\n    \"transform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Transform\"\n        },\n        {\n          \"description\": \"Specifies an asset transform property. A transform contains a mathematical expression that maps a property's data points from one form to another, such as a unit conversion from Celsius to Fahrenheit.\"\n        }\n      ]\n    },\n    \"metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metric\"\n        },\n        {\n          \"description\": \"Specifies an asset metric property. A metric contains a mathematical expression that uses aggregate functions to process all input data points over a time interval and output a single data point, such\
  \ as to calculate the average hourly temperature.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-property-type-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: PropertyType
---
