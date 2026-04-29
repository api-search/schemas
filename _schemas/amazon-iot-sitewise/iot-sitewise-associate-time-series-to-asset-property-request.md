---
description: AssociateTimeSeriesToAssetPropertyRequest schema
layout: schema
name: AssociateTimeSeriesToAssetPropertyRequest
properties_list:
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-associate-time-series-to-asset-property-request-schema.json
slug: iot-sitewise-associate-time-series-to-asset-property-request
source_filename: iot-sitewise-associate-time-series-to-asset-property-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-associate-time-series-to-asset-property-request-schema.json\",\n  \"title\": \"AssociateTimeSeriesToAssetPropertyRequest\",\n  \"description\": \"AssociateTimeSeriesToAssetPropertyRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique case-sensitive identifier that you can provide to ensure the idempotency of the request. Don't reuse this client token if a new idempotent request is required.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-associate-time-series-to-asset-property-request-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssociateTimeSeriesToAssetPropertyRequest
---
