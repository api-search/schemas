---
description: The output from the DescribeThing operation.
layout: schema
name: DescribeThingResponse
properties_list:
- description: ''
  name: defaultClientId
  type: object
- description: ''
  name: thingName
  type: object
- description: ''
  name: thingId
  type: object
- description: ''
  name: thingArn
  type: object
- description: ''
  name: thingTypeName
  type: object
- description: ''
  name: attributes
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: billingGroupName
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-thing-response-schema.json
slug: iot-core-describe-thing-response
source_filename: iot-core-describe-thing-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-thing-response-schema.json\",\n  \"title\": \"DescribeThingResponse\",\n  \"description\": \"The output from the DescribeThing operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientId\"\n        },\n        {\n          \"description\": \"<p>The default MQTT client ID. For a typical device, the thing name is also used as the default MQTT client ID. Although we don\\u2019t require a mapping between a thing's registry name and its use of MQTT client IDs, certificates, or shadow state, we recommend that you choose a thing name and use it as the MQTT client ID for the registry and the Device Shadow service.</p> <p>This lets you better organize your IoT fleet without removing\
  \ the flexibility of the underlying device certificate model or shadows.</p>\"\n        }\n      ]\n    },\n    \"thingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingName\"\n        },\n        {\n          \"description\": \"The name of the thing.\"\n        }\n      ]\n    },\n    \"thingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingId\"\n        },\n        {\n          \"description\": \"The ID of the thing to describe.\"\n        }\n      ]\n    },\n    \"thingArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingArn\"\n        },\n        {\n          \"description\": \"The ARN of the thing to describe.\"\n        }\n      ]\n    },\n    \"thingTypeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeName\"\n        },\n        {\n          \"description\": \"The thing type name.\"\n        }\n      ]\n    },\n    \"attributes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attributes\"\n        },\n        {\n          \"description\": \"The thing attributes.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"<p>The current version of the thing record in the registry.</p> <note> <p>To avoid unintentional changes to the information in the registry, you can pass the version information in the <code>expectedVersion</code> parameter of the <code>UpdateThing</code> and <code>DeleteThing</code> calls.</p> </note>\"\n        }\n      ]\n    },\n    \"billingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BillingGroupName\"\n        },\n        {\n          \"description\": \"The name of the billing group the thing belongs to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-thing-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeThingResponse
---
