---
description: <a href="https://www.w3.org/auto/wg/wiki/Vehicle_Signal_Specification_(VSS)/Vehicle_Data_Spec">Vehicle Signal Specification (VSS)</a> is a precise language used to describe and model signals in vehicle networks. The JSON file collects signal specificiations in a VSS format.
layout: schema
name: FormattedVss
properties_list:
- description: ''
  name: vssJson
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-formatted-vss-schema.json
slug: iot-fleetwise-formatted-vss
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-formatted-vss-schema.json\",\n  \"title\": \"FormattedVss\",\n  \"description\": \" <a href=\\\"https://www.w3.org/auto/wg/wiki/Vehicle_Signal_Specification_(VSS)/Vehicle_Data_Spec\\\">Vehicle Signal Specification (VSS)</a> is a precise language used to describe and model signals in vehicle networks. The JSON file collects signal specificiations in a VSS format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vssJson\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Provides the VSS in JSON format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-formatted-vss-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: FormattedVss
---
