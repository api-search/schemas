---
description: <p>Contains information about a deployment's policy that defines when components are safe to update.</p> <p>Each component on a device can report whether or not it's ready to update. After a component and its dependencies are ready, they can apply the update in the deployment. You can configure whether or not the deployment notifies components of an update and waits for a response. You specify the amount of time each component has to respond to the update notification.</p>
layout: schema
name: DeploymentComponentUpdatePolicy
properties_list:
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: action
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-deployment-component-update-policy-schema.json
slug: iot-greengrass-deployment-component-update-policy
source_filename: iot-greengrass-deployment-component-update-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-component-update-policy-schema.json\",\n  \"title\": \"DeploymentComponentUpdatePolicy\",\n  \"description\": \"<p>Contains information about a deployment's policy that defines when components are safe to update.</p> <p>Each component on a device can report whether or not it's ready to update. After a component and its dependencies are ready, they can apply the update in the deployment. You can configure whether or not the deployment notifies components of an update and waits for a response. You specify the amount of time each component has to respond to the update notification.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n      \
  \  {\n          \"description\": \"<p>The amount of time in seconds that each component on a device has to report that it's safe to update. If the component waits for longer than this timeout, then the deployment proceeds on the device.</p> <p>Default: <code>60</code> </p>\"\n        }\n      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentComponentUpdatePolicyAction\"\n        },\n        {\n          \"description\": \"<p>Whether or not to notify components and wait for components to become safe to update. Choose from the following options:</p> <ul> <li> <p> <code>NOTIFY_COMPONENTS</code> \\u2013 The deployment notifies each component before it stops and updates that component. Components can use the <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/interprocess-communication.html#ipc-operation-subscribetocomponentupdates\\\">SubscribeToComponentUpdates</a> IPC operation to receive these notifications.\
  \ Then, components can respond with the <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/interprocess-communication.html#ipc-operation-defercomponentupdate\\\">DeferComponentUpdate</a> IPC operation. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/create-deployments.html\\\">Create deployments</a> in the <i>IoT Greengrass V2 Developer Guide</i>.</p> </li> <li> <p> <code>SKIP_NOTIFY_COMPONENTS</code> \\u2013 The deployment doesn't notify components or wait for them to be safe to update.</p> </li> </ul> <p>Default: <code>NOTIFY_COMPONENTS</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-component-update-policy-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DeploymentComponentUpdatePolicy
---
