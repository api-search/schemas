---
description: <p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>An allowed instance type for a game server group. All game server groups must have at least two instance types defined for it. Amazon GameLift FleetIQ periodically evaluates each defined instance type for viability. It then updates the Auto Scaling group with the list of viable instance types.</p>
layout: schema
name: InstanceDefinition
properties_list:
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: WeightedCapacity
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-instance-definition-schema.json
slug: gamelift-instance-definition
source_filename: gamelift-instance-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-instance-definition-schema.json\",\n  \"title\": \"InstanceDefinition\",\n  \"description\": \"<p> <b>This data type is used with the Amazon GameLift FleetIQ and game server groups.</b> </p> <p>An allowed instance type for a game server group. All game server groups must have at least two instance types defined for it. Amazon GameLift FleetIQ periodically evaluates each defined instance type for viability. It then updates the Auto Scaling group with the list of viable instance types.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameServerGroupInstanceType\"\n        },\n        {\n          \"description\": \"An Amazon EC2 instance type designation.\"\n        }\n      ]\n    },\n    \"\
  WeightedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WeightedCapacity\"\n        },\n        {\n          \"description\": \"Instance weighting that indicates how much this instance type contributes to the total capacity of a game server group. Instance weights are used by Amazon GameLift FleetIQ to calculate the instance type's cost per unit hour and better identify the most cost-effective options. For detailed information on weighting instance capacity, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-instance-weighting.html\\\">Instance Weighting</a> in the <i>Amazon Elastic Compute Cloud Auto Scaling User Guide</i>. Default value is \\\"1\\\".\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-instance-definition-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: InstanceDefinition
---
