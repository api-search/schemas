---
description: UpdatePricingPlanRequest schema
layout: schema
name: UpdatePricingPlanRequest
properties_list:
- description: ''
  name: pricingMode
  type: object
- description: ''
  name: bundleNames
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-pricing-plan-request-schema.json
slug: iot-twinmaker-update-pricing-plan-request
source_filename: iot-twinmaker-update-pricing-plan-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-pricing-plan-request-schema.json\",\n  \"title\": \"UpdatePricingPlanRequest\",\n  \"description\": \"UpdatePricingPlanRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pricingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingMode\"\n        },\n        {\n          \"description\": \"The pricing mode.\"\n        }\n      ]\n    },\n    \"bundleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingBundles\"\n        },\n        {\n          \"description\": \"The bundle names.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pricingMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-pricing-plan-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdatePricingPlanRequest
---
