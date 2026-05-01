---
description: Contains information about system resource limits that the IoT Greengrass Core software applies to a component's processes. For more information, see <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-system-resource-limits">Configure system resource limits for components</a>.
layout: schema
name: SystemResourceLimits
properties_list:
- description: ''
  name: memory
  type: object
- description: ''
  name: cpus
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-system-resource-limits-schema.json
slug: iot-greengrass-system-resource-limits
source_filename: iot-greengrass-system-resource-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-system-resource-limits-schema.json\",\n  \"title\": \"SystemResourceLimits\",\n  \"description\": \"Contains information about system resource limits that the IoT Greengrass Core software applies to a component's processes. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-system-resource-limits\\\">Configure system resource limits for components</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Memory\"\n        },\n        {\n          \"description\": \"The maximum amount of RAM, expressed in kilobytes, that a component's processes can use on the core device.\"\n        }\n      ]\n  \
  \  },\n    \"cpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CPU\"\n        },\n        {\n          \"description\": \"The maximum amount of CPU time that a component's processes can use on the core device. A core device's total CPU time is equivalent to the device's number of CPU cores. For example, on a core device with 4 CPU cores, you can set this value to <code>2</code> to limit the component's processes to 50 percent usage of each CPU core. On a device with 1 CPU core, you can set this value to <code>0.25</code> to limit the component's processes to 25 percent usage of the CPU. If you set this value to a number greater than the number of CPU cores, the IoT Greengrass Core software doesn't limit the component's CPU usage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-system-resource-limits-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: SystemResourceLimits
---
