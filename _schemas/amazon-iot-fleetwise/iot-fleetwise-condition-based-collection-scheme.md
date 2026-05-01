---
description: Information about a collection scheme that uses a simple logical expression to recognize what data to collect.
layout: schema
name: ConditionBasedCollectionScheme
properties_list:
- description: ''
  name: expression
  type: object
- description: ''
  name: minimumTriggerIntervalMs
  type: object
- description: ''
  name: triggerMode
  type: object
- description: ''
  name: conditionLanguageVersion
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-condition-based-collection-scheme-schema.json
slug: iot-fleetwise-condition-based-collection-scheme
source_filename: iot-fleetwise-condition-based-collection-scheme-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-condition-based-collection-scheme-schema.json\",\n  \"title\": \"ConditionBasedCollectionScheme\",\n  \"description\": \"Information about a collection scheme that uses a simple logical expression to recognize what data to collect.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/eventExpression\"\n        },\n        {\n          \"description\": \"The logical expression used to recognize what data to collect. For example, <code>$variable.Vehicle.OutsideAirTemperature &gt;= 105.0</code>.\"\n        }\n      ]\n    },\n    \"minimumTriggerIntervalMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/uint32\"\n        },\n        {\n          \"description\":\
  \ \"<p>The minimum duration of time between two triggering events to collect data, in milliseconds.</p> <note> <p>If a signal changes often, you might want to collect data at a slower rate.</p> </note>\"\n        }\n      ]\n    },\n    \"triggerMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerMode\"\n        },\n        {\n          \"description\": \"Whether to collect data for all triggering events (<code>ALWAYS</code>). Specify (<code>RISING_EDGE</code>), or specify only when the condition first evaluates to false. For example, triggering on \\\"AirbagDeployed\\\"; Users aren't interested on triggering when the airbag is already exploded; they only care about the change from not deployed =&gt; deployed.\"\n        }\n      ]\n    },\n    \"conditionLanguageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/languageVersion\"\n        },\n        {\n          \"description\": \"Specifies the version of the\
  \ conditional expression language.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"expression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-condition-based-collection-scheme-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ConditionBasedCollectionScheme
---
