---
description: AssetPropertySummaries schema
layout: schema
name: AssetPropertySummaries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-property-summaries-schema.json
slug: iot-sitewise-asset-property-summaries
source_filename: iot-sitewise-asset-property-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-summaries-schema.json\",\n  \"title\": \"AssetPropertySummaries\",\n  \"description\": \"AssetPropertySummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \"The ID of the property.\"\n          }\n        ]\n      },\n      \"alias\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyAlias\"\n          },\n          {\n            \"description\": \"The alias that identifies the property, such as an OPC-UA server data stream path (for example, <code>/company/windfarm/3/turbine/7/temperature</code>). For more information,\
  \ see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/connect-data-streams.html\\\">Mapping industrial data streams to asset properties</a> in the <i>IoT SiteWise User Guide</i>.\"\n          }\n        ]\n      },\n      \"unit\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PropertyUnit\"\n          },\n          {\n            \"description\": \" The unit of measure (such as Newtons or RPM) of the asset property. \"\n          }\n        ]\n      },\n      \"notification\": {\n        \"$ref\": \"#/components/schemas/PropertyNotification\"\n      },\n      \"assetCompositeModelId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ID\"\n          },\n          {\n            \"description\": \" The ID of the composite model that contains the asset property. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains a summary of a property associated with an asset.\"\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-property-summaries-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetPropertySummaries
---
