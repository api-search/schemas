---
description: UpdatePricingPlanResponse schema
layout: schema
name: UpdatePricingPlanResponse
properties_list:
- description: ''
  name: currentPricingPlan
  type: object
- description: ''
  name: pendingPricingPlan
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-pricing-plan-response-schema.json
slug: iot-twinmaker-update-pricing-plan-response
source_filename: iot-twinmaker-update-pricing-plan-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-pricing-plan-response-schema.json\",\n  \"title\": \"UpdatePricingPlanResponse\",\n  \"description\": \"UpdatePricingPlanResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPricingPlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingPlan\"\n        },\n        {\n          \"description\": \"Update the current pricing plan.\"\n        }\n      ]\n    },\n    \"pendingPricingPlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingPlan\"\n        },\n        {\n          \"description\": \"Update the pending pricing plan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"currentPricingPlan\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-pricing-plan-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdatePricingPlanResponse
---
