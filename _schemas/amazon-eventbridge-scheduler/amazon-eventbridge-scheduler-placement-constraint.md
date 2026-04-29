---
description: An object representing a constraint on task placement.
layout: schema
name: PlacementConstraint
properties_list:
- description: ''
  name: expression
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-placement-constraint-schema.json
slug: amazon-eventbridge-scheduler-placement-constraint
source_filename: amazon-eventbridge-scheduler-placement-constraint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-placement-constraint-schema.json\",\n  \"title\": \"PlacementConstraint\",\n  \"description\": \"An object representing a constraint on task placement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementConstraintExpression\"\n        },\n        {\n          \"description\": \"A cluster query language expression to apply to the constraint. You cannot specify an expression if the constraint type is <code>distinctInstance</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/latest/developerguide/cluster-query-language.html\\\">Cluster query language</a> in the <i>Amazon ECS Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"type\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementConstraintType\"\n        },\n        {\n          \"description\": \"The type of constraint. Use <code>distinctInstance</code> to ensure that each task in a particular group is running on a different container instance. Use <code>memberOf</code> to restrict the selection to a group of valid candidates.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-placement-constraint-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: PlacementConstraint
---
