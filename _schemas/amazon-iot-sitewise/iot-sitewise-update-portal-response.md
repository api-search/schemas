---
description: UpdatePortalResponse schema
layout: schema
name: UpdatePortalResponse
properties_list:
- description: ''
  name: portalStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-update-portal-response-schema.json
slug: iot-sitewise-update-portal-response
source_filename: iot-sitewise-update-portal-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-update-portal-response-schema.json\",\n  \"title\": \"UpdatePortalResponse\",\n  \"description\": \"UpdatePortalResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portalStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalStatus\"\n        },\n        {\n          \"description\": \"The status of the portal, which contains a state (<code>UPDATING</code> after successfully calling this operation) and any error message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"portalStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-update-portal-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: UpdatePortalResponse
---
