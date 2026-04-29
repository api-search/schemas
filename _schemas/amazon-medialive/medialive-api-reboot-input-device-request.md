---
description: A request to reboot an AWS Elemental device.
layout: schema
name: RebootInputDeviceRequest
properties_list:
- description: ''
  name: Force
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-reboot-input-device-request-schema.json
slug: medialive-api-reboot-input-device-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reboot-input-device-request-schema.json\",\n  \"title\": \"RebootInputDeviceRequest\",\n  \"description\": \"A request to reboot an AWS Elemental device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Force\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RebootInputDeviceForce\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"force\"\n          },\n          \"description\": \"Force a reboot of an input device. If the device is streaming, it will stop streaming and begin rebooting within a few seconds of sending the command. If the device was streaming prior to the reboot, the device will resume streaming when the reboot completes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-reboot-input-device-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: RebootInputDeviceRequest
---
