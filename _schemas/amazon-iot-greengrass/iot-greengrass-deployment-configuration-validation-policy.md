---
description: Contains information about how long a component on a core device can validate its configuration updates before it times out. Components can use the <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/interprocess-communication.html#ipc-operation-subscribetovalidateconfigurationupdates">SubscribeToValidateConfigurationUpdates</a> IPC operation to receive notifications when a deployment specifies a configuration update. Then, components can respond with the <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/interprocess-communication.html#ipc-operation-sendconfigurationvalidityreport">SendConfigurationValidityReport</a> IPC operation. For more information, see <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/create-deployments.html">Create deployments</a> in the <i>IoT Greengrass V2 Developer Guide</i>.
layout: schema
name: DeploymentConfigurationValidationPolicy
properties_list:
- description: ''
  name: timeoutInSeconds
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-deployment-configuration-validation-policy-schema.json
slug: iot-greengrass-deployment-configuration-validation-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-configuration-validation-policy-schema.json\",\n  \"title\": \"DeploymentConfigurationValidationPolicy\",\n  \"description\": \"Contains information about how long a component on a core device can validate its configuration updates before it times out. Components can use the <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/interprocess-communication.html#ipc-operation-subscribetovalidateconfigurationupdates\\\">SubscribeToValidateConfigurationUpdates</a> IPC operation to receive notifications when a deployment specifies a configuration update. Then, components can respond with the <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/interprocess-communication.html#ipc-operation-sendconfigurationvalidityreport\\\">SendConfigurationValidityReport</a>\
  \ IPC operation. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/create-deployments.html\\\">Create deployments</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n        {\n          \"description\": \"<p>The amount of time in seconds that a component can validate its configuration updates. If the validation time exceeds this timeout, then the deployment proceeds for the device.</p> <p>Default: <code>30</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-configuration-validation-policy-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DeploymentConfigurationValidationPolicy
---
