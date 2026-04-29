---
description: InstalledComponentList schema
layout: schema
name: InstalledComponentList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-installed-component-list-schema.json
slug: iot-greengrass-installed-component-list
source_filename: iot-greengrass-installed-component-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-installed-component-list-schema.json\",\n  \"title\": \"InstalledComponentList\",\n  \"description\": \"InstalledComponentList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"componentName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentNameString\"\n          },\n          {\n            \"description\": \"The name of the component.\"\n          }\n        ]\n      },\n      \"componentVersion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentVersionString\"\n          },\n          {\n            \"description\": \"The version of the component.\"\n          }\n        ]\n      },\n      \"lifecycleState\": {\n        \"allOf\": [\n\
  \          {\n            \"$ref\": \"#/components/schemas/InstalledComponentLifecycleState\"\n          },\n          {\n            \"description\": \"The lifecycle state of the component.\"\n          }\n        ]\n      },\n      \"lifecycleStateDetails\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LifecycleStateDetails\"\n          },\n          {\n            \"description\": \"A detailed response about the lifecycle state of the component that explains the reason why a component has an error or is broken.\"\n          }\n        ]\n      },\n      \"isRoot\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IsRoot\"\n          },\n          {\n            \"description\": \"Whether or not the component is a root component.\"\n          }\n        ]\n      },\n      \"lastStatusChangeTimestamp\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n \
  \         {\n            \"description\": \"<p>The status of how current the data is.</p> <p>This response is based off of component state changes. The status reflects component disruptions and deployments. If a component only sees a configuration update during a deployment, it might not undergo a state change and this status would not be updated.</p>\"\n          }\n        ]\n      },\n      \"lastReportedTimestamp\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"<p>The last time the Greengrass core device sent a message containing a component's state to the Amazon Web Services Cloud.</p> <p>A component does not need to see a state change for this field to update.</p>\"\n          }\n        ]\n      },\n      \"lastInstallationSource\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"\
  description\": \"<p>The most recent deployment source that brought the component to the Greengrass core device. For a thing group deployment or thing deployment, the source will be the The ID of the deployment. and for local deployments it will be <code>LOCAL</code>.</p> <note> <p>Any deployment will attempt to reinstall currently broken components on the device, which will update the last installation source.</p> </note>\"\n          }\n        ]\n      },\n      \"lifecycleStatusCodes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/InstalledComponentLifecycleStatusCodeList\"\n          },\n          {\n            \"description\": \"<p>The status codes that indicate the reason for failure whenever the <code>lifecycleState</code> has an error or is in a broken state.</p> <note> <p>Greengrass nucleus v2.8.0 or later is required to get an accurate <code>lifecycleStatusCodes</code> response. This response can be inaccurate in earlier Greengrass nucleus\
  \ versions.</p> </note>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a component on a Greengrass core device.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-installed-component-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: InstalledComponentList
---
