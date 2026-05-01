---
description: Contains details for a gateway that runs on IoT Greengrass V2. To create a gateway that runs on IoT Greengrass V2, you must deploy the IoT SiteWise Edge component to your gateway device. Your <a href="https://docs.aws.amazon.com/greengrass/v2/developerguide/device-service-role.html">Greengrass device role</a> must use the <code>AWSIoTSiteWiseEdgeAccess</code> policy. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/userguide/sw-gateways.html">Using IoT SiteWise at the edge</a> in the <i>IoT SiteWise User Guide</i>.
layout: schema
name: GreengrassV2
properties_list:
- description: ''
  name: coreDeviceThingName
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-greengrass-v2-schema.json
slug: iot-sitewise-greengrass-v2
source_filename: iot-sitewise-greengrass-v2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-greengrass-v2-schema.json\",\n  \"title\": \"GreengrassV2\",\n  \"description\": \"Contains details for a gateway that runs on IoT Greengrass V2. To create a gateway that runs on IoT Greengrass V2, you must deploy the IoT SiteWise Edge component to your gateway device. Your <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/device-service-role.html\\\">Greengrass device role</a> must use the <code>AWSIoTSiteWiseEdgeAccess</code> policy. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/sw-gateways.html\\\">Using IoT SiteWise at the edge</a> in the <i>IoT SiteWise User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coreDeviceThingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoreDeviceThingName\"\
  \n        },\n        {\n          \"description\": \"The name of the IoT thing for your IoT Greengrass V2 core device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"coreDeviceThingName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-greengrass-v2-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: GreengrassV2
---
