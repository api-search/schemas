---
description: The identifer of the input.
layout: schema
name: InputIdentifier
properties_list:
- description: ''
  name: iotEventsInputIdentifier
  type: object
- description: ''
  name: iotSiteWiseInputIdentifier
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-input-identifier-schema.json
slug: iot-events-input-identifier
source_filename: iot-events-input-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-identifier-schema.json\",\n  \"title\": \"InputIdentifier\",\n  \"description\": \" The identifer of the input. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iotEventsInputIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotEventsInputIdentifier\"\n        },\n        {\n          \"description\": \" The identifier of the input routed to AWS IoT Events. \"\n        }\n      ]\n    },\n    \"iotSiteWiseInputIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotSiteWiseInputIdentifier\"\n        },\n        {\n          \"description\": \" The identifer of the input routed from AWS IoT SiteWise. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-identifier-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: InputIdentifier
---
