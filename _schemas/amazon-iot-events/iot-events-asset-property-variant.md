---
description: <p>A structure that contains an asset property value. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_Variant.html">Variant</a> in the <i>AWS IoT SiteWise API Reference</i>.</p> <p>You must use expressions for all parameters in <code>AssetPropertyVariant</code>. The expressions accept literals, operators, functions, references, and substitution templates.</p> <p class="title"> <b>Examples</b> </p> <ul> <li> <p>For literal values, the expressions must contain single quotes. For example, the value for the <code>integerValue</code> parameter can be <code>'100'</code>.</p> </li> <li> <p>For references, you must specify either variables or parameters. For example, the value for the <code>booleanValue</code> parameter can be <code>$variable.offline</code>.</p> </li> <li> <p>For a substitution template, you must use <code>${}</code>, and the template must be in single quotes. A substitution template can also contain a combination
  of literals, operators, functions, references, and substitution templates. </p> <p>In the following example, the value for the <code>doubleValue</code> parameter uses a substitution template. </p> <p> <code>'${$input.TemperatureInput.sensorData.temperature * 6 / 5 + 32}'</code> </p> </li> </ul> <p>For more information, see <a href="https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-expressions.html">Expressions</a> in the <i>AWS IoT Events Developer Guide</i>.</p> <p>You must specify one of the following value types, depending on the <code>dataType</code> of the specified asset property. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_AssetProperty.html">AssetProperty</a> in the <i>AWS IoT SiteWise API Reference</i>.</p>
layout: schema
name: AssetPropertyVariant
properties_list:
- description: ''
  name: stringValue
  type: object
- description: ''
  name: integerValue
  type: object
- description: ''
  name: doubleValue
  type: object
- description: ''
  name: booleanValue
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-asset-property-variant-schema.json
slug: iot-events-asset-property-variant
source_filename: iot-events-asset-property-variant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-asset-property-variant-schema.json\",\n  \"title\": \"AssetPropertyVariant\",\n  \"description\": \"<p>A structure that contains an asset property value. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_Variant.html\\\">Variant</a> in the <i>AWS IoT SiteWise API Reference</i>.</p> <p>You must use expressions for all parameters in <code>AssetPropertyVariant</code>. The expressions accept literals, operators, functions, references, and substitution templates.</p> <p class=\\\"title\\\"> <b>Examples</b> </p> <ul> <li> <p>For literal values, the expressions must contain single quotes. For example, the value for the <code>integerValue</code> parameter can be <code>'100'</code>.</p> </li> <li> <p>For references, you must specify either variables\
  \ or parameters. For example, the value for the <code>booleanValue</code> parameter can be <code>$variable.offline</code>.</p> </li> <li> <p>For a substitution template, you must use <code>${}</code>, and the template must be in single quotes. A substitution template can also contain a combination of literals, operators, functions, references, and substitution templates. </p> <p>In the following example, the value for the <code>doubleValue</code> parameter uses a substitution template. </p> <p> <code>'${$input.TemperatureInput.sensorData.temperature * 6 / 5 + 32}'</code> </p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-expressions.html\\\">Expressions</a> in the <i>AWS IoT Events Developer Guide</i>.</p> <p>You must specify one of the following value types, depending on the <code>dataType</code> of the specified asset property. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_AssetProperty.html\\\
  \">AssetProperty</a> in the <i>AWS IoT SiteWise API Reference</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stringValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyStringValue\"\n        },\n        {\n          \"description\": \"The asset property value is a string. You must use an expression, and the evaluated result should be a string.\"\n        }\n      ]\n    },\n    \"integerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyIntegerValue\"\n        },\n        {\n          \"description\": \"The asset property value is an integer. You must use an expression, and the evaluated result should be an integer.\"\n        }\n      ]\n    },\n    \"doubleValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyDoubleValue\"\n        },\n        {\n          \"description\": \"The asset property value is a double. You must use an expression,\
  \ and the evaluated result should be a double.\"\n        }\n      ]\n    },\n    \"booleanValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyBooleanValue\"\n        },\n        {\n          \"description\": \"The asset property value is a Boolean value that must be <code>'TRUE'</code> or <code>'FALSE'</code>. You must use an expression, and the evaluated result should be a Boolean value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-asset-property-variant-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AssetPropertyVariant
---
