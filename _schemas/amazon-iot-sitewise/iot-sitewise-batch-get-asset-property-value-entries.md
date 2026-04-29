---
description: BatchGetAssetPropertyValueEntries schema
layout: schema
name: BatchGetAssetPropertyValueEntries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-get-asset-property-value-entries-schema.json
slug: iot-sitewise-batch-get-asset-property-value-entries
source_filename: iot-sitewise-batch-get-asset-property-value-entries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-entries-schema.json\",\n  \"title\": \"BatchGetAssetPropertyValueEntries\",\n  \"description\": \"BatchGetAssetPropertyValueEntries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"entryId\"\n    ],\n    \"properties\": {\n      \"entryId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EntryId\"\n          },\n          {\n            \"description\": \"The ID of the entry.\"\n          }\n        ]\n      },\n      \"assetId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the asset in which the asset property was created.\"\n          }\n        ]\n\
  \      },\n      \"propertyId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the asset property.\"\n          }\n        ]\n      },\n      \"propertyAlias\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetPropertyAlias\"\n          },\n          {\n            \"description\": \"The alias that identifies the property, such as an OPC-UA server data stream path (for example, <code>/company/windfarm/3/turbine/7/temperature</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/connect-data-streams.html\\\">Mapping industrial data streams to asset properties</a> in the <i>IoT SiteWise User Guide</i>.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"<p>Contains information for an asset property value entry that is associated with the <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_BatchGetAssetPropertyValue.html\\\
  \">BatchGetAssetPropertyValue</a> API.</p> <p>To identify an asset property, you must specify one of the following:</p> <ul> <li> <p>The <code>assetId</code> and <code>propertyId</code> of an asset property.</p> </li> <li> <p>A <code>propertyAlias</code>, which is a data stream alias (for example, <code>/company/windfarm/3/turbine/7/temperature</code>). To define an asset property's alias, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/APIReference/API_UpdateAssetProperty.html\\\">UpdateAssetProperty</a>.</p> </li> </ul>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-get-asset-property-value-entries-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchGetAssetPropertyValueEntries
---
