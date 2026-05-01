---
description: ListInstalledComponentsResponse schema
layout: schema
name: ListInstalledComponentsResponse
properties_list:
- description: ''
  name: installedComponents
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-list-installed-components-response-schema.json
slug: iot-greengrass-list-installed-components-response
source_filename: iot-greengrass-list-installed-components-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-installed-components-response-schema.json\",\n  \"title\": \"ListInstalledComponentsResponse\",\n  \"description\": \"ListInstalledComponentsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"installedComponents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstalledComponentList\"\n        },\n        {\n          \"description\": \"<p>A list that summarizes each component on the core device.</p> <note> <p>Greengrass nucleus v2.7.0 or later is required to get an accurate <code>lastStatusChangeTimestamp</code> response. This response can be inaccurate in earlier Greengrass nucleus versions.</p> </note> <note> <p>Greengrass nucleus v2.8.0 or later is required to get an accurate <code>lastInstallationSource</code> and <code>lastReportedTimestamp</code>\
  \ response. This response can be inaccurate or null in earlier Greengrass nucleus versions.</p> </note>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextTokenString\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-installed-components-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ListInstalledComponentsResponse
---
