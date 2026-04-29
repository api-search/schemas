---
description: Information about the pricing bundle.
layout: schema
name: BundleInformation
properties_list:
- description: ''
  name: bundleNames
  type: object
- description: ''
  name: pricingTier
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-bundle-information-schema.json
slug: iot-twinmaker-bundle-information
source_filename: iot-twinmaker-bundle-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-bundle-information-schema.json\",\n  \"title\": \"BundleInformation\",\n  \"description\": \"Information about the pricing bundle.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bundleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingBundles\"\n        },\n        {\n          \"description\": \"The bundle names.\"\n        }\n      ]\n    },\n    \"pricingTier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingTier\"\n        },\n        {\n          \"description\": \"The pricing tier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bundleNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-bundle-information-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: BundleInformation
---
