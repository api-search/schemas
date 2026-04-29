---
description: ComponentDeploymentSpecifications schema
layout: schema
name: ComponentDeploymentSpecifications
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-deployment-specifications-schema.json
slug: iot-greengrass-component-deployment-specifications
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-deployment-specifications-schema.json\",\n  \"title\": \"ComponentDeploymentSpecifications\",\n  \"description\": \"ComponentDeploymentSpecifications schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"componentVersion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentVersionString\"\n          },\n          {\n            \"description\": \"The version of the component.\"\n          }\n        ]\n      },\n      \"configurationUpdate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentConfigurationUpdate\"\n          },\n          {\n            \"description\": \"The configuration updates to deploy for the component.\
  \ You can define <i>reset</i> updates and <i>merge</i> updates. A reset updates the keys that you specify to the default configuration for the component. A merge updates the core device's component configuration with the keys and values that you specify. The IoT Greengrass Core software applies reset updates before it applies merge updates. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/update-component-configurations.html\\\">Update component configurations</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n          }\n        ]\n      },\n      \"runWith\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentRunWith\"\n          },\n          {\n            \"description\": \"The system user and group that the IoT Greengrass Core software uses to run component processes on the core device. If you omit this parameter, the IoT Greengrass Core software uses the system user and group that you configure\
  \ for the core device. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-user\\\">Configure the user and group that run components</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a component to deploy.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-deployment-specifications-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentDeploymentSpecifications
---
