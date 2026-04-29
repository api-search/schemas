---
description: The asset model property identifer of the input routed from AWS IoT SiteWise.
layout: schema
name: IotSiteWiseAssetModelPropertyIdentifier
properties_list:
- description: ''
  name: assetModelId
  type: object
- description: ''
  name: propertyId
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-iot-site-wise-asset-model-property-identifier-schema.json
slug: iot-events-iot-site-wise-asset-model-property-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-site-wise-asset-model-property-identifier-schema.json\",\n  \"title\": \"IotSiteWiseAssetModelPropertyIdentifier\",\n  \"description\": \" The asset model property identifer of the input routed from AWS IoT SiteWise. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetModelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetModelId\"\n        },\n        {\n          \"description\": \" The ID of the AWS IoT SiteWise asset model. \"\n        }\n      ]\n    },\n    \"propertyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetPropertyId\"\n        },\n        {\n          \"description\": \" The ID of the AWS IoT SiteWise asset property. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"assetModelId\"\
  ,\n    \"propertyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-iot-site-wise-asset-model-property-identifier-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: IotSiteWiseAssetModelPropertyIdentifier
---
