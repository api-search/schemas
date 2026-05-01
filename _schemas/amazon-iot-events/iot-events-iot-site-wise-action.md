---
description: <p>Sends information about the detector model instance and the event that triggered the action to a specified asset property in AWS IoT SiteWise.</p> <p>You must use expressions for all parameters in <code>IotSiteWiseAction</code>. The expressions accept literals, operators, functions, references, and substitutions templates.</p> <p class="title"> <b>Examples</b> </p> <ul> <li> <p>For literal values, the expressions must contain single quotes. For example, the value for the <code>propertyAlias</code> parameter can be <code>'/company/windfarm/3/turbine/7/temperature'</code>.</p> </li> <li> <p>For references, you must specify either variables or input values. For example, the value for the <code>assetId</code> parameter can be <code>$input.TurbineInput.assetId1</code>.</p> </li> <li> <p>For a substitution template, you must use <code>${}</code>, and the template must be in single quotes. A substitution template can also contain a combination of literals, operators, functions,
  references, and substitution templates.</p> <p>In the following example, the value for the <code>propertyAlias</code> parameter uses a substitution template. </p> <p> <code>'company/windfarm/${$input.TemperatureInput.sensorData.windfarmID}/turbine/ ${$input.TemperatureInput.sensorData.turbineID}/temperature'</code> </p> </li> </ul> <p>You must specify either <code>propertyAlias</code> or both <code>assetId</code> and <code>propertyId</code> to identify the target asset property in AWS IoT SiteWise.</p> <p>For more information, see <a href="https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-expressions.html">Expressions</a> in the <i>AWS IoT Events Developer Guide</i>.</p>
layout: schema
name: IotSiteWiseAction
properties_list:
- description: ''
  name: entryId
  type: object
- description: ''
  name: assetId
  type: object
- description: ''
  name: propertyId
  type: object
- description: ''
  name: propertyAlias
  type: object
- description: ''
  name: propertyValue
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-iot-site-wise-action-schema.json
slug: iot-events-iot-site-wise-action
source_filename: iot-events-iot-site-wise-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-site-wise-action-schema.json\",\n  \"title\": \"IotSiteWiseAction\",\n  \"description\": \"<p>Sends information about the detector model instance and the event that triggered the action to a specified asset property in AWS IoT SiteWise.</p> <p>You must use expressions for all parameters in <code>IotSiteWiseAction</code>. The expressions accept literals, operators, functions, references, and substitutions templates.</p> <p class=\\\"title\\\"> <b>Examples</b> </p> <ul> <li> <p>For literal values, the expressions must contain single quotes. For example, the value for the <code>propertyAlias</code> parameter can be <code>'/company/windfarm/3/turbine/7/temperature'</code>.</p> </li> <li> <p>For references, you must specify either variables or input values. For example, the value for the <code>assetId</code>\
  \ parameter can be <code>$input.TurbineInput.assetId1</code>.</p> </li> <li> <p>For a substitution template, you must use <code>${}</code>, and the template must be in single quotes. A substitution template can also contain a combination of literals, operators, functions, references, and substitution templates.</p> <p>In the following example, the value for the <code>propertyAlias</code> parameter uses a substitution template. </p> <p> <code>'company/windfarm/${$input.TemperatureInput.sensorData.windfarmID}/turbine/ ${$input.TemperatureInput.sensorData.turbineID}/temperature'</code> </p> </li> </ul> <p>You must specify either <code>propertyAlias</code> or both <code>assetId</code> and <code>propertyId</code> to identify the target asset property in AWS IoT SiteWise.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/iotevents-expressions.html\\\">Expressions</a> in the <i>AWS IoT Events Developer Guide</i>.</p>\",\n  \"type\": \"object\"\
  ,\n  \"properties\": {\n    \"entryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyEntryId\"\n        },\n        {\n          \"description\": \"A unique identifier for this entry. You can use the entry ID to track which data entry causes an error in case of failure. The default is a new unique identifier.\"\n        }\n      ]\n    },\n    \"assetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetId\"\n        },\n        {\n          \"description\": \"The ID of the asset that has the specified property.\"\n        }\n      ]\n    },\n    \"propertyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyId\"\n        },\n        {\n          \"description\": \"The ID of the asset property.\"\n        }\n      ]\n    },\n    \"propertyAlias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyAlias\"\n        },\n       \
  \ {\n          \"description\": \"The alias of the asset property.\"\n        }\n      ]\n    },\n    \"propertyValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyValue\"\n        },\n        {\n          \"description\": \"The value to send to the asset property. This value contains timestamp, quality, and value (TQV) information. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-site-wise-action-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: IotSiteWiseAction
---
