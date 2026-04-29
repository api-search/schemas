---
description: PutScalingPolicyInput schema from Amazon GameLift API
layout: schema
name: PutScalingPolicyInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: FleetId
  type: object
- description: ''
  name: ScalingAdjustment
  type: object
- description: ''
  name: ScalingAdjustmentType
  type: object
- description: ''
  name: Threshold
  type: object
- description: ''
  name: ComparisonOperator
  type: object
- description: ''
  name: EvaluationPeriods
  type: object
- description: ''
  name: MetricName
  type: object
- description: ''
  name: PolicyType
  type: object
- description: ''
  name: TargetConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-put-scaling-policy-input-schema.json
slug: gamelift-put-scaling-policy-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-put-scaling-policy-input-schema.json\",\n  \"title\": \"PutScalingPolicyInput\",\n  \"description\": \"PutScalingPolicyInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a fleet's scaling policy. Policy names do not need to be unique. A fleet can have only one scaling policy with the same name.\"\n        }\n      ]\n    },\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to apply this policy to. You can use\
  \ either the fleet ID or ARN value. The fleet cannot be in any of the following statuses: ERROR or DELETING.\"\n        }\n      ]\n    },\n    \"ScalingAdjustment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Amount of adjustment to make, based on the scaling adjustment type.\"\n        }\n      ]\n    },\n    \"ScalingAdjustmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingAdjustmentType\"\n        },\n        {\n          \"description\": \"<p>The type of adjustment to make to a fleet's instance count:</p> <ul> <li> <p> <b>ChangeInCapacity</b> -- add (or subtract) the scaling adjustment value from the current instance count. Positive values scale up while negative values scale down.</p> </li> <li> <p> <b>ExactCapacity</b> -- set the instance count to the scaling adjustment value.</p> </li> <li> <p> <b>PercentChangeInCapacity</b> -- increase or\
  \ reduce the current instance count by the scaling adjustment, read as a percentage. Positive values scale up while negative values scale down; for example, a value of \\\"-10\\\" scales the fleet down by 10%.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Threshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Metric value used to trigger a scaling event.\"\n        }\n      ]\n    },\n    \"ComparisonOperator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComparisonOperatorType\"\n        },\n        {\n          \"description\": \"Comparison operator to use when measuring the metric against the threshold value.\"\n        }\n      ]\n    },\n    \"EvaluationPeriods\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"Length of time (in minutes) the metric\
  \ must be at or beyond the threshold before a scaling event is triggered.\"\n        }\n      ]\n    },\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"<p>Name of the Amazon GameLift-defined metric that is used to trigger a scaling adjustment. For detailed descriptions of fleet metrics, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/monitoring-cloudwatch.html\\\">Monitor Amazon GameLift with Amazon CloudWatch</a>. </p> <ul> <li> <p> <b>ActivatingGameSessions</b> -- Game sessions in the process of being created.</p> </li> <li> <p> <b>ActiveGameSessions</b> -- Game sessions that are currently running.</p> </li> <li> <p> <b>ActiveInstances</b> -- Fleet instances that are currently running at least one game session.</p> </li> <li> <p> <b>AvailableGameSessions</b> -- Additional game sessions that fleet could host simultaneously, given current capacity.</p>\
  \ </li> <li> <p> <b>AvailablePlayerSessions</b> -- Empty player slots in currently active game sessions. This includes game sessions that are not currently accepting players. Reserved player slots are not included.</p> </li> <li> <p> <b>CurrentPlayerSessions</b> -- Player slots in active game sessions that are being used by a player or are reserved for a player. </p> </li> <li> <p> <b>IdleInstances</b> -- Active instances that are currently hosting zero game sessions. </p> </li> <li> <p> <b>PercentAvailableGameSessions</b> -- Unused percentage of the total number of game sessions that a fleet could host simultaneously, given current capacity. Use this metric for a target-based scaling policy.</p> </li> <li> <p> <b>PercentIdleInstances</b> -- Percentage of the total number of active instances that are hosting zero game sessions.</p> </li> <li> <p> <b>QueueDepth</b> -- Pending game session placement requests, in any queue, where the current fleet is the top-priority destination.</p> </li>\
  \ <li> <p> <b>WaitTime</b> -- Current wait time for pending game session placement requests, in any queue, where the current fleet is the top-priority destination. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"PolicyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyType\"\n        },\n        {\n          \"description\": \"The type of scaling policy to create. For a target-based policy, set the parameter <i>MetricName</i> to 'PercentAvailableGameSessions' and specify a <i>TargetConfiguration</i>. For a rule-based policy set the following parameters: <i>MetricName</i>, <i>ComparisonOperator</i>, <i>Threshold</i>, <i>EvaluationPeriods</i>, <i>ScalingAdjustmentType</i>, and <i>ScalingAdjustment</i>.\"\n        }\n      ]\n    },\n    \"TargetConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetConfiguration\"\n        },\n        {\n          \"description\": \"An object that contains settings\
  \ for a target-based scaling policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"FleetId\",\n    \"MetricName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-put-scaling-policy-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: PutScalingPolicyInput
---
