---
description: The pricing plan.
layout: schema
name: PricingPlan
properties_list:
- description: ''
  name: billableEntityCount
  type: object
- description: ''
  name: bundleInformation
  type: object
- description: ''
  name: effectiveDateTime
  type: object
- description: ''
  name: pricingMode
  type: object
- description: ''
  name: updateDateTime
  type: object
- description: ''
  name: updateReason
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-pricing-plan-schema.json
slug: iot-twinmaker-pricing-plan
source_filename: iot-twinmaker-pricing-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-pricing-plan-schema.json\",\n  \"title\": \"PricingPlan\",\n  \"description\": \"The pricing plan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billableEntityCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The billable entity count.\"\n        }\n      ]\n    },\n    \"bundleInformation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleInformation\"\n        },\n        {\n          \"description\": \"The pricing plan's bundle information.\"\n        }\n      ]\n    },\n    \"effectiveDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The effective\
  \ date and time of the pricing plan.\"\n        }\n      ]\n    },\n    \"pricingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingMode\"\n        },\n        {\n          \"description\": \"The pricing mode.\"\n        }\n      ]\n    },\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The set date and time for updating a pricing plan.\"\n        }\n      ]\n    },\n    \"updateReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateReason\"\n        },\n        {\n          \"description\": \"The update reason for changing a pricing plan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"effectiveDateTime\",\n    \"pricingMode\",\n    \"updateDateTime\",\n    \"updateReason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-pricing-plan-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PricingPlan
---
