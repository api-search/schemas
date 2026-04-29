---
description: Rule that controls how a fleet is scaled. Scaling policies are uniquely identified by the combination of name and fleet ID.
layout: schema
name: ScalingPolicy
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ScalingAdjustment
  type: object
- description: ''
  name: ScalingAdjustmentType
  type: object
- description: ''
  name: ComparisonOperator
  type: object
- description: ''
  name: Threshold
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
- description: ''
  name: UpdateStatus
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-scaling-policy-schema.json
slug: gamelift-scaling-policy
source_filename: gamelift-scaling-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-scaling-policy-schema.json\",\n  \"title\": \"ScalingPolicy\",\n  \"description\": \"Rule that controls how a fleet is scaled. Scaling policies are uniquely identified by the combination of name and fleet ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that is associated with this scaling policy.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that\
  \ is assigned to a Amazon GameLift fleet resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a fleet's scaling policy. Policy names do not need to be unique.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingStatusType\"\n        },\n        {\n          \"description\": \"<p>Current status of the scaling policy. The scaling policy can be in force only when in an <code>ACTIVE</code> status. Scaling policies can be suspended for individual fleets. If the policy is suspended for a fleet, the policy status does not change.</p> <ul> <li> <p> <b>ACTIVE</b>\
  \ -- The scaling policy can be used for auto-scaling a fleet.</p> </li> <li> <p> <b>UPDATE_REQUESTED</b> -- A request to update the scaling policy has been received.</p> </li> <li> <p> <b>UPDATING</b> -- A change is being made to the scaling policy.</p> </li> <li> <p> <b>DELETE_REQUESTED</b> -- A request to delete the scaling policy has been received.</p> </li> <li> <p> <b>DELETING</b> -- The scaling policy is being deleted.</p> </li> <li> <p> <b>DELETED</b> -- The scaling policy has been deleted.</p> </li> <li> <p> <b>ERROR</b> -- An error occurred in creating the policy. It should be removed and recreated.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ScalingAdjustment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Amount of adjustment to make, based on the scaling adjustment type.\"\n        }\n      ]\n    },\n    \"ScalingAdjustmentType\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/ScalingAdjustmentType\"\n        },\n        {\n          \"description\": \"<p>The type of adjustment to make to a fleet's instance count.</p> <ul> <li> <p> <b>ChangeInCapacity</b> -- add (or subtract) the scaling adjustment value from the current instance count. Positive values scale up while negative values scale down.</p> </li> <li> <p> <b>ExactCapacity</b> -- set the instance count to the scaling adjustment value.</p> </li> <li> <p> <b>PercentChangeInCapacity</b> -- increase or reduce the current instance count by the scaling adjustment, read as a percentage. Positive values scale up while negative values scale down.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ComparisonOperator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComparisonOperatorType\"\n        },\n        {\n          \"description\": \"Comparison operator to use when measuring a metric against the threshold value.\"\n        }\n      ]\n\
  \    },\n    \"Threshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Metric value used to trigger a scaling event.\"\n        }\n      ]\n    },\n    \"EvaluationPeriods\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"Length of time (in minutes) the metric must be at or beyond the threshold before a scaling event is triggered.\"\n        }\n      ]\n    },\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"<p>Name of the Amazon GameLift-defined metric that is used to trigger a scaling adjustment. For detailed descriptions of fleet metrics, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/monitoring-cloudwatch.html\\\">Monitor Amazon GameLift with Amazon\
  \ CloudWatch</a>. </p> <ul> <li> <p> <b>ActivatingGameSessions</b> -- Game sessions in the process of being created.</p> </li> <li> <p> <b>ActiveGameSessions</b> -- Game sessions that are currently running.</p> </li> <li> <p> <b>ActiveInstances</b> -- Fleet instances that are currently running at least one game session.</p> </li> <li> <p> <b>AvailableGameSessions</b> -- Additional game sessions that fleet could host simultaneously, given current capacity.</p> </li> <li> <p> <b>AvailablePlayerSessions</b> -- Empty player slots in currently active game sessions. This includes game sessions that are not currently accepting players. Reserved player slots are not included.</p> </li> <li> <p> <b>CurrentPlayerSessions</b> -- Player slots in active game sessions that are being used by a player or are reserved for a player. </p> </li> <li> <p> <b>IdleInstances</b> -- Active instances that are currently hosting zero game sessions. </p> </li> <li> <p> <b>PercentAvailableGameSessions</b> -- Unused\
  \ percentage of the total number of game sessions that a fleet could host simultaneously, given current capacity. Use this metric for a target-based scaling policy.</p> </li> <li> <p> <b>PercentIdleInstances</b> -- Percentage of the total number of active instances that are hosting zero game sessions.</p> </li> <li> <p> <b>QueueDepth</b> -- Pending game session placement requests, in any queue, where the current fleet is the top-priority destination.</p> </li> <li> <p> <b>WaitTime</b> -- Current wait time for pending game session placement requests, in any queue, where the current fleet is the top-priority destination. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"PolicyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyType\"\n        },\n        {\n          \"description\": \"The type of scaling policy to create. For a target-based policy, set the parameter <i>MetricName</i> to 'PercentAvailableGameSessions' and specify a <i>TargetConfiguration</i>.\
  \ For a rule-based policy set the following parameters: <i>MetricName</i>, <i>ComparisonOperator</i>, <i>Threshold</i>, <i>EvaluationPeriods</i>, <i>ScalingAdjustmentType</i>, and <i>ScalingAdjustment</i>.\"\n        }\n      ]\n    },\n    \"TargetConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetConfiguration\"\n        },\n        {\n          \"description\": \"An object that contains settings for a target-based scaling policy.\"\n        }\n      ]\n    },\n    \"UpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationUpdateStatus\"\n        },\n        {\n          \"description\": \"The current status of the fleet's scaling policies in a requested fleet location. The status <code>PENDING_UPDATE</code> indicates that an update was requested for the fleet but has not yet been completed for the location.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \" The fleet location. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-scaling-policy-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ScalingPolicy
---
