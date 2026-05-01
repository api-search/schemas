---
description: The details of a capacity provider strategy. To learn more, see <a href="https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CapacityProviderStrategyItem.html">CapacityProviderStrategyItem</a> in the Amazon ECS API Reference.
layout: schema
name: CapacityProviderStrategyItem
properties_list:
- description: ''
  name: base
  type: object
- description: ''
  name: capacityProvider
  type: object
- description: ''
  name: weight
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-capacity-provider-strategy-item-schema.json
slug: amazon-eventbridge-pipes-capacity-provider-strategy-item
source_filename: amazon-eventbridge-pipes-capacity-provider-strategy-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-capacity-provider-strategy-item-schema.json\",\n  \"title\": \"CapacityProviderStrategyItem\",\n  \"description\": \"The details of a capacity provider strategy. To learn more, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CapacityProviderStrategyItem.html\\\">CapacityProviderStrategyItem</a> in the Amazon ECS API Reference.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityProviderStrategyItemBase\"\n        },\n        {\n          \"description\": \"The base value designates how many tasks, at a minimum, to run on the specified capacity provider. Only one capacity provider in a capacity provider strategy can have a base defined. If no value\
  \ is specified, the default value of 0 is used. \"\n        }\n      ]\n    },\n    \"capacityProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityProvider\"\n        },\n        {\n          \"description\": \"The short name of the capacity provider.\"\n        }\n      ]\n    },\n    \"weight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityProviderStrategyItemWeight\"\n        },\n        {\n          \"description\": \"The weight value designates the relative percentage of the total number of tasks launched that should use the specified capacity provider. The weight value is taken into consideration after the base value, if defined, is satisfied.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"capacityProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-capacity-provider-strategy-item-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: CapacityProviderStrategyItem
---
