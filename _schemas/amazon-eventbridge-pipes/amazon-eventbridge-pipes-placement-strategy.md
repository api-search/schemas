---
description: The task placement strategy for a task or service. To learn more, see <a href="https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-strategies.html">Task Placement Strategies</a> in the Amazon Elastic Container Service Service Developer Guide.
layout: schema
name: PlacementStrategy
properties_list:
- description: ''
  name: field
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-placement-strategy-schema.json
slug: amazon-eventbridge-pipes-placement-strategy
source_filename: amazon-eventbridge-pipes-placement-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-placement-strategy-schema.json\",\n  \"title\": \"PlacementStrategy\",\n  \"description\": \"The task placement strategy for a task or service. To learn more, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-strategies.html\\\">Task Placement Strategies</a> in the Amazon Elastic Container Service Service Developer Guide.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementStrategyField\"\n        },\n        {\n          \"description\": \"The field to apply the placement strategy against. For the spread placement strategy, valid values are instanceId (or host, which has the same effect), or any platform or custom attribute that is\
  \ applied to a container instance, such as attribute:ecs.availability-zone. For the binpack placement strategy, valid values are cpu and memory. For the random placement strategy, this field is not used. \"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementStrategyType\"\n        },\n        {\n          \"description\": \"The type of placement strategy. The random placement strategy randomly places tasks on available candidates. The spread placement strategy spreads placement across available candidates evenly based on the field parameter. The binpack strategy places tasks on available candidates that have the least available amount of the resource that is specified with the field parameter. For example, if you binpack on memory, a task is placed on the instance with the least amount of remaining memory (but still enough to run the task). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-placement-strategy-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PlacementStrategy
---
