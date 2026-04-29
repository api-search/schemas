---
description: The identifer of the input routed from AWS IoT SiteWise.
layout: schema
name: IotSiteWiseInputIdentifier
properties_list:
- description: ''
  name: iotSiteWiseAssetModelPropertyIdentifier
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-iot-site-wise-input-identifier-schema.json
slug: iot-events-iot-site-wise-input-identifier
source_filename: iot-events-iot-site-wise-input-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-site-wise-input-identifier-schema.json\",\n  \"title\": \"IotSiteWiseInputIdentifier\",\n  \"description\": \" The identifer of the input routed from AWS IoT SiteWise. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iotSiteWiseAssetModelPropertyIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotSiteWiseAssetModelPropertyIdentifier\"\n        },\n        {\n          \"description\": \" The identifier of the AWS IoT SiteWise asset model property. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-site-wise-input-identifier-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: IotSiteWiseInputIdentifier
---
