---
description: Contains information about a deployment's update to a component's configuration on Greengrass core devices. For more information, see <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/update-component-configurations.html">Update component configurations</a> in the <i>IoT Greengrass V2 Developer Guide</i>.
layout: schema
name: ComponentConfigurationUpdate
properties_list:
- description: ''
  name: merge
  type: object
- description: ''
  name: reset
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-configuration-update-schema.json
slug: iot-greengrass-component-configuration-update
source_filename: iot-greengrass-component-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-configuration-update-schema.json\",\n  \"title\": \"ComponentConfigurationUpdate\",\n  \"description\": \"Contains information about a deployment's update to a component's configuration on Greengrass core devices. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/update-component-configurations.html\\\">Update component configurations</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentConfigurationString\"\n        },\n        {\n          \"description\": \"A serialized JSON string that contains the configuration object to merge to target devices. The core device merges this configuration\
  \ with the component's existing configuration. If this is the first time a component deploys on a device, the core device merges this configuration with the component's default configuration. This means that the core device keeps it's existing configuration for keys and values that you don't specify in this object. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/update-component-configurations.html#merge-configuration-update\\\">Merge configuration updates</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"reset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentConfigurationPathList\"\n        },\n        {\n          \"description\": \"The list of configuration nodes to reset to default values on target devices. Use JSON pointers to specify each node to reset. JSON pointers start with a forward slash (<code>/</code>) and use forward slashes to separate the key for\
  \ each level in the object. For more information, see the <a href=\\\"https://tools.ietf.org/html/rfc6901\\\">JSON pointer specification</a> and <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/update-component-configurations.html#reset-configuration-update\\\">Reset configuration updates</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-configuration-update-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentConfigurationUpdate
---
