---
description: <p>Describes a Amazon GameLift fleet of game hosting resources.</p> <p> <b>Related actions</b> </p>
layout: schema
name: FleetAttributes
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: FleetType
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: TerminationTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: BuildId
  type: object
- description: ''
  name: BuildArn
  type: object
- description: ''
  name: ScriptId
  type: object
- description: ''
  name: ScriptArn
  type: object
- description: ''
  name: ServerLaunchPath
  type: object
- description: ''
  name: ServerLaunchParameters
  type: object
- description: ''
  name: LogPaths
  type: object
- description: ''
  name: NewGameSessionProtectionPolicy
  type: object
- description: ''
  name: OperatingSystem
  type: object
- description: ''
  name: ResourceCreationLimitPolicy
  type: object
- description: ''
  name: MetricGroups
  type: object
- description: ''
  name: StoppedActions
  type: object
- description: ''
  name: InstanceRoleArn
  type: object
- description: ''
  name: CertificateConfiguration
  type: object
- description: ''
  name: ComputeType
  type: object
- description: ''
  name: AnywhereConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-fleet-attributes-schema.json
slug: gamelift-fleet-attributes
source_filename: gamelift-fleet-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-fleet-attributes-schema.json\",\n  \"title\": \"FleetAttributes\",\n  \"description\": \"<p>Describes a Amazon GameLift fleet of game hosting resources.</p> <p> <b>Related actions</b> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift fleet resource and uniquely\
  \ identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>. In a GameLift fleet ARN, the resource ID matches the <code>FleetId</code> value.\"\n        }\n      ]\n    },\n    \"FleetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetType\"\n        },\n        {\n          \"description\": \"Indicates whether to use On-Demand or Spot instances for this fleet. By default, this property is set to <code>ON_DEMAND</code>. Learn more about when to use <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-ec2-instances.html#gamelift-ec2-instances-spot\\\"> On-Demand versus Spot Instances</a>. This property cannot be changed after the fleet is created.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceType\"\n        },\n        {\n        \
  \  \"description\": \"The Amazon EC2 instance type that determines the computing resources of each instance in the fleet. Instance type defines the CPU, memory, storage, and networking capacity. See <a href=\\\"http://aws.amazon.com/ec2/instance-types/\\\">Amazon Elastic Compute Cloud Instance Types</a> for detailed descriptions.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A human-readable description of the fleet.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a fleet. Fleet names do not need to be unique.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"TerminationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was terminated. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetStatus\"\n        },\n        {\n          \"description\": \"<p>Current status of the fleet. Possible fleet statuses include the following:</p> <ul> <li> <p> <b>NEW</b> -- A new fleet has been defined and desired instances is set to 1. </p> </li> <li> <p> <b>DOWNLOADING/VALIDATING/BUILDING/ACTIVATING</b>\
  \ -- Amazon GameLift is setting up the new fleet, creating new instances with the game build or Realtime script and starting server processes.</p> </li> <li> <p> <b>ACTIVE</b> -- Hosts can now accept game sessions.</p> </li> <li> <p> <b>ERROR</b> -- An error occurred when downloading, validating, building, or activating the fleet.</p> </li> <li> <p> <b>DELETING</b> -- Hosts are responding to a delete fleet request.</p> </li> <li> <p> <b>TERMINATED</b> -- The fleet no longer exists.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"BuildId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildId\"\n        },\n        {\n          \"description\": \"A unique identifier for the build resource that is deployed on instances in this fleet.\"\n        }\n      ]\n    },\n    \"BuildArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (<a href=\\\
  \"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) associated with the Amazon GameLift build resource that is deployed on instances in this fleet. In a GameLift build ARN, the resource ID matches the <code>BuildId</code> value.\"\n        }\n      ]\n    },\n    \"ScriptId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptId\"\n        },\n        {\n          \"description\": \"A unique identifier for the Realtime script resource that is deployed on instances in this fleet.\"\n        }\n      ]\n    },\n    \"ScriptArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) associated with the GameLift script resource that is deployed on instances in this fleet. In a GameLift script ARN, the resource ID matches the\
  \ <code>ScriptId</code> value.\"\n        }\n      ]\n    },\n    \"ServerLaunchPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchPathStringModel\"\n        },\n        {\n          \"description\": \" <b>This parameter is no longer used.</b> Server launch paths are now defined using the fleet's <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/RuntimeConfiguration.html\\\">RuntimeConfiguration</a> . Requests that use this parameter instead continue to be valid.\"\n        }\n      ]\n    },\n    \"ServerLaunchParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchParametersStringModel\"\n        },\n        {\n          \"description\": \" <b>This parameter is no longer used.</b> Server launch parameters are now defined using the fleet's runtime configuration . Requests that use this parameter instead continue to be valid.\"\n        }\n      ]\n    },\n    \"LogPaths\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \" <b>This parameter is no longer used.</b> Game session log paths are now defined using the Amazon GameLift server API <code>ProcessReady()</code> <code>logParameters</code>. See more information in the <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api-ref.html#gamelift-sdk-server-api-ref-dataypes-process\\\">Server API Reference</a>. \"\n        }\n      ]\n    },\n    \"NewGameSessionProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtectionPolicy\"\n        },\n        {\n          \"description\": \"<p>The type of game session protection to set on all new instances that are started in the fleet.</p> <ul> <li> <p> <b>NoProtection</b> -- The game session can be terminated during a scale-down event.</p> </li> <li> <p> <b>FullProtection</b> -- If the game session is in an\
  \ <code>ACTIVE</code> status, it cannot be terminated during a scale-down event.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"The operating system of the fleet's computing resources. A fleet's operating system is determined by the OS of the build or script that is deployed on this fleet.\"\n        }\n      ]\n    },\n    \"ResourceCreationLimitPolicy\": {\n      \"$ref\": \"#/components/schemas/ResourceCreationLimitPolicy\"\n    },\n    \"MetricGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricGroupList\"\n        },\n        {\n          \"description\": \"Name of a metric group that metrics for this fleet are added to. In Amazon CloudWatch, you can view aggregated metrics for fleets that are in a metric group. A fleet can be included in only one metric group at a time.\"\
  \n        }\n      ]\n    },\n    \"StoppedActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetActionList\"\n        },\n        {\n          \"description\": \"A list of fleet activity that has been suspended using <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_StopFleetActions.html\\\">StopFleetActions</a> . This includes fleet auto-scaling.\"\n        }\n      ]\n    },\n    \"InstanceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A unique identifier for an IAM role that manages access to your Amazon Web Services services. With an instance role ARN set, any application that runs on an instance in this fleet can assume the role, including install scripts, server processes, and daemons (background processes). Create a role or look up a role's ARN by using the <a href=\\\"https://console.aws.amazon.com/iam/\\\"\
  >IAM dashboard</a> in the Amazon Web Services Management Console. Learn more about using on-box credentials for your game servers at <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-resources.html\\\"> Access external resources from a game server</a>.\"\n        }\n      ]\n    },\n    \"CertificateConfiguration\": {\n      \"$ref\": \"#/components/schemas/CertificateConfiguration\"\n    },\n    \"ComputeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n        },\n        {\n          \"description\": \"The type of compute resource used to host your game servers. You can use your own compute resources with Amazon GameLift Anywhere or use Amazon EC2 instances with managed Amazon GameLift.\"\n        }\n      ]\n    },\n    \"AnywhereConfiguration\": {\n      \"$ref\": \"#/components/schemas/AnywhereConfiguration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-fleet-attributes-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: FleetAttributes
---
