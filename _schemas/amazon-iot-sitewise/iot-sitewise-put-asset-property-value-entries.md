---
description: PutAssetPropertyValueEntries schema
layout: schema
name: PutAssetPropertyValueEntries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-put-asset-property-value-entries-schema.json
slug: iot-sitewise-put-asset-property-value-entries
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-put-asset-property-value-entries-schema.json\",\n  \"title\": \"PutAssetPropertyValueEntries\",\n  \"description\": \"PutAssetPropertyValueEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"entryId\",\n      \"propertyValues\"\n    ],\n    \"properties\": {\n      \"entryId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntryId\"\n          },\n          {\n            \"description\": \"The user specified ID for the entry. You can use this ID to identify which entries failed.\"\n          }\n        ]\n      },\n      \"assetId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of\
  \ the asset to update.\"\n          }\n        ]\n      },\n      \"propertyId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the asset property for this entry.\"\n          }\n        ]\n      },\n      \"propertyAlias\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetPropertyAlias\"\n          },\n          {\n            \"description\": \"The alias that identifies the property, such as an OPC-UA server data stream path (for example, <code>/company/windfarm/3/turbine/7/temperature</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/connect-data-streams.html\\\">Mapping industrial data streams to asset properties</a> in the <i>IoT SiteWise User Guide</i>.\"\n          }\n        ]\n      },\n      \"propertyValues\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetPropertyValues\"\
  \n          },\n          {\n            \"description\": \"The list of property values to upload. You can specify up to 10 <code>propertyValues</code> array elements. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains a list of value updates for an asset property in the list of asset entries consumed by the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchPutAssetPropertyValue.html\\\">BatchPutAssetPropertyValue</a> API operation.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-put-asset-property-value-entries-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: PutAssetPropertyValueEntries
---
