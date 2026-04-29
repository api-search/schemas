---
description: <p>A structure that contains value information. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_AssetPropertyValue.html">AssetPropertyValue</a> in the <i>AWS IoT SiteWise API Reference</i>.</p> <p>You must use expressions for all parameters in <code>AssetPropertyValue</code>. The expressions accept literals, operators, functions, references, and substitution templates.</p> <p class="title"> <b>Examples</b> </p> <ul> <li> <p>For literal values, the expressions must contain single quotes. For example, the value for the <code>quality</code> parameter can be <code>'GOOD'</code>.</p> </li> <li> <p>For references, you must specify either variables or input values. For example, the value for the <code>quality</code> parameter can be <code>$input.TemperatureInput.sensorData.quality</code>.</p> </li> </ul> <p>For more information, see <a href="https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-expressions.html">Expressions</a>
  in the <i>AWS IoT Events Developer Guide</i>.</p>
layout: schema
name: AssetPropertyValue
properties_list:
- description: ''
  name: value
  type: object
- description: ''
  name: timestamp
  type: object
- description: ''
  name: quality
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-asset-property-value-schema.json
slug: iot-events-asset-property-value
source_filename: iot-events-asset-property-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-asset-property-value-schema.json\",\n  \"title\": \"AssetPropertyValue\",\n  \"description\": \"<p>A structure that contains value information. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_AssetPropertyValue.html\\\">AssetPropertyValue</a> in the <i>AWS IoT SiteWise API Reference</i>.</p> <p>You must use expressions for all parameters in <code>AssetPropertyValue</code>. The expressions accept literals, operators, functions, references, and substitution templates.</p> <p class=\\\"title\\\"> <b>Examples</b> </p> <ul> <li> <p>For literal values, the expressions must contain single quotes. For example, the value for the <code>quality</code> parameter can be <code>'GOOD'</code>.</p> </li> <li> <p>For references, you must specify either\
  \ variables or input values. For example, the value for the <code>quality</code> parameter can be <code>$input.TemperatureInput.sensorData.quality</code>.</p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-expressions.html\\\">Expressions</a> in the <i>AWS IoT Events Developer Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyVariant\"\n        },\n        {\n          \"description\": \"The value to send to an asset property.\"\n        }\n      ]\n    },\n    \"timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyTimestamp\"\n        },\n        {\n          \"description\": \"The timestamp associated with the asset property value. The default is the current event time.\"\n        }\n      ]\n    },\n    \"quality\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/AssetPropertyQuality\"\n        },\n        {\n          \"description\": \"The quality of the asset property value. The value must be <code>'GOOD'</code>, <code>'BAD'</code>, or <code>'UNCERTAIN'</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-asset-property-value-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AssetPropertyValue
---
