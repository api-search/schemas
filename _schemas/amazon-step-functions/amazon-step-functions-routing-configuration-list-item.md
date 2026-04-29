---
description: Contains details about the routing configuration of a state machine alias. In a routing configuration, you define an array of objects that specify up to two state machine versions. You also specify the percentage of traffic to be routed to each version.
layout: schema
name: RoutingConfigurationListItem
properties_list:
- description: ''
  name: stateMachineVersionArn
  type: object
- description: ''
  name: weight
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-routing-configuration-list-item-schema.json
slug: amazon-step-functions-routing-configuration-list-item
source_filename: amazon-step-functions-routing-configuration-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-routing-configuration-list-item-schema.json\",\n  \"title\": \"RoutingConfigurationListItem\",\n  \"description\": \"Contains details about the routing configuration of a state machine alias. In a routing configuration, you define an array of objects that specify up to two state machine versions. You also specify the percentage of traffic to be routed to each version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) that identifies one or two state machine versions defined in the routing configuration.</p> <p>If you specify the ARN of a second version, it must belong to the same\
  \ state machine as the first version.</p>\"\n        }\n      ]\n    },\n    \"weight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionWeight\"\n        },\n        {\n          \"description\": \"The percentage of traffic you want to route to the second state machine version. The sum of the weights in the routing configuration must be equal to 100.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineVersionArn\",\n    \"weight\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-routing-configuration-list-item-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: RoutingConfigurationListItem
---
