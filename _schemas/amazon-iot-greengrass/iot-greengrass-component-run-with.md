---
description: Contains information system user and group that the IoT Greengrass Core software uses to run component processes on the core device. For more information, see <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-user">Configure the user and group that run components</a> in the <i>IoT Greengrass V2 Developer Guide</i>.
layout: schema
name: ComponentRunWith
properties_list:
- description: ''
  name: posixUser
  type: object
- description: ''
  name: systemResourceLimits
  type: object
- description: ''
  name: windowsUser
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-run-with-schema.json
slug: iot-greengrass-component-run-with
source_filename: iot-greengrass-component-run-with-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-run-with-schema.json\",\n  \"title\": \"ComponentRunWith\",\n  \"description\": \"Contains information system user and group that the IoT Greengrass Core software uses to run component processes on the core device. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-user\\\">Configure the user and group that run components</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"posixUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The POSIX system user and, optionally, group to use to run this component on Linux core\
  \ devices. The user, and group if specified, must exist on each Linux core device. Specify the user and group separated by a colon (<code>:</code>) in the following format: <code>user:group</code>. The group is optional. If you don't specify a group, the IoT Greengrass Core software uses the primary user for the group.</p> <p>If you omit this parameter, the IoT Greengrass Core software uses the default system user and group that you configure on the Greengrass nucleus component. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-user\\\">Configure the user and group that run components</a>.</p>\"\n        }\n      ]\n    },\n    \"systemResourceLimits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SystemResourceLimits\"\n        },\n        {\n          \"description\": \"<p>The system resource limits to apply to this component's process on the core device.\
  \ IoT Greengrass currently supports this feature on only Linux core devices.</p> <p>If you omit this parameter, the IoT Greengrass Core software uses the default system resource limits that you configure on the Greengrass nucleus component. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-system-resource-limits\\\">Configure system resource limits for components</a>.</p>\"\n        }\n      ]\n    },\n    \"windowsUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The Windows user to use to run this component on Windows core devices. The user must exist on each Windows core device, and its name and password must be in the LocalSystem account's Credentials Manager instance.</p> <p>If you omit this parameter, the IoT Greengrass Core software uses the default Windows user that you configure\
  \ on the Greengrass nucleus component. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/configure-greengrass-core-v2.html#configure-component-user\\\">Configure the user and group that run components</a>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-run-with-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentRunWith
---
