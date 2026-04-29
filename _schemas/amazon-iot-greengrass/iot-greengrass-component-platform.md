---
description: Contains information about a platform that a component supports.
layout: schema
name: ComponentPlatform
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: attributes
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-platform-schema.json
slug: iot-greengrass-component-platform
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-platform-schema.json\",\n  \"title\": \"ComponentPlatform\",\n  \"description\": \"Contains information about a platform that a component supports.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The friendly name of the platform. This name helps you identify the platform.</p> <p>If you omit this parameter, IoT Greengrass creates a friendly name from the <code>os</code> and <code>architecture</code> of the platform.</p>\"\n        }\n      ]\n    },\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlatformAttributesMap\"\n        },\n        {\n          \"description\"\
  : \"A dictionary of attributes for the platform. The IoT Greengrass Core software defines the <code>os</code> and <code>architecture</code> by default. You can specify additional platform attributes for a core device when you deploy the Greengrass nucleus component. For more information, see the <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/greengrass-nucleus-component.html\\\">Greengrass nucleus component</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-platform-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentPlatform
---
