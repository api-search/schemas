---
description: AssetRelationshipSummaries schema
layout: schema
name: AssetRelationshipSummaries
properties_list: []
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-asset-relationship-summaries-schema.json
slug: iot-sitewise-asset-relationship-summaries
source_filename: iot-sitewise-asset-relationship-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-relationship-summaries-schema.json\",\n  \"title\": \"AssetRelationshipSummaries\",\n  \"description\": \"AssetRelationshipSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"relationshipType\"\n    ],\n    \"properties\": {\n      \"hierarchyInfo\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetHierarchyInfo\"\n          },\n          {\n            \"description\": \"<p>The assets that are related through an asset hierarchy.</p> <p>This object is present if the <code>relationshipType</code> is <code>HIERARCHY</code>.</p>\"\n          }\n        ]\n      },\n      \"relationshipType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AssetRelationshipType\"\
  \n          },\n          {\n            \"description\": \"<p>The relationship type of the assets in this relationship. This value is one of the following:</p> <ul> <li> <p> <code>HIERARCHY</code> \\u2013 The assets are related through an asset hierarchy. If you specify this relationship type, this asset relationship includes the <code>hierarchyInfo</code> object.</p> </li> </ul>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about assets that are related to one another.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-asset-relationship-summaries-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: AssetRelationshipSummaries
---
