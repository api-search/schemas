---
description: An object representing a constraint on task placement. To learn more, see <a href="https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-constraints.html">Task Placement Constraints</a> in the Amazon Elastic Container Service Developer Guide.
layout: schema
name: PlacementConstraint
properties_list:
- description: ''
  name: expression
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-placement-constraint-schema.json
slug: amazon-eventbridge-pipes-placement-constraint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-placement-constraint-schema.json\",\n  \"title\": \"PlacementConstraint\",\n  \"description\": \"An object representing a constraint on task placement. To learn more, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-placement-constraints.html\\\">Task Placement Constraints</a> in the Amazon Elastic Container Service Developer Guide.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementConstraintExpression\"\n        },\n        {\n          \"description\": \"A cluster query language expression to apply to the constraint. You cannot specify an expression if the constraint type is <code>distinctInstance</code>. To learn more, see <a href=\\\
  \"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cluster-query-language.html\\\">Cluster Query Language</a> in the Amazon Elastic Container Service Developer Guide. \"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementConstraintType\"\n        },\n        {\n          \"description\": \"The type of constraint. Use distinctInstance to ensure that each task in a particular group is running on a different container instance. Use memberOf to restrict the selection to a group of valid candidates. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-placement-constraint-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PlacementConstraint
---
