---
description: CreateFleetInput schema from Amazon GameLift API
layout: schema
name: CreateFleetInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: BuildId
  type: object
- description: ''
  name: ScriptId
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
  name: EC2InstanceType
  type: object
- description: ''
  name: EC2InboundPermissions
  type: object
- description: ''
  name: NewGameSessionProtectionPolicy
  type: object
- description: ''
  name: RuntimeConfiguration
  type: object
- description: ''
  name: ResourceCreationLimitPolicy
  type: object
- description: ''
  name: MetricGroups
  type: object
- description: ''
  name: PeerVpcAwsAccountId
  type: object
- description: ''
  name: PeerVpcId
  type: object
- description: ''
  name: FleetType
  type: object
- description: ''
  name: InstanceRoleArn
  type: object
- description: ''
  name: CertificateConfiguration
  type: object
- description: ''
  name: Locations
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ComputeType
  type: object
- description: ''
  name: AnywhereConfiguration
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-fleet-input-schema.json
slug: gamelift-create-fleet-input
source_filename: gamelift-create-fleet-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-input-schema.json\",\n  \"title\": \"CreateFleetInput\",\n  \"description\": \"CreateFleetInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a fleet. Fleet names do not need to be unique.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A description for the fleet.\"\n        }\n      ]\n    },\n    \"BuildId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIdOrArn\"\
  \n        },\n        {\n          \"description\": \"The unique identifier for a custom game server build to be deployed on fleet instances. You can use either the build ID or ARN. The build must be uploaded to Amazon GameLift and in <code>READY</code> status. This fleet property cannot be changed later.\"\n        }\n      ]\n    },\n    \"ScriptId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptIdOrArn\"\n        },\n        {\n          \"description\": \"The unique identifier for a Realtime configuration script to be deployed on fleet instances. You can use either the script ID or ARN. Scripts must be uploaded to Amazon GameLift prior to creating the fleet. This fleet property cannot be changed later.\"\n        }\n      ]\n    },\n    \"ServerLaunchPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchPathStringModel\"\n        },\n        {\n          \"description\": \" <b>This parameter is no longer used.</b>\
  \ Specify a server launch path using the <code>RuntimeConfiguration</code> parameter. Requests that use this parameter instead continue to be valid.\"\n        }\n      ]\n    },\n    \"ServerLaunchParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchParametersStringModel\"\n        },\n        {\n          \"description\": \" <b>This parameter is no longer used.</b> Specify server launch parameters using the <code>RuntimeConfiguration</code> parameter. Requests that use this parameter instead continue to be valid.\"\n        }\n      ]\n    },\n    \"LogPaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \" <b>This parameter is no longer used.</b> To specify where Amazon GameLift should store log files once a server process shuts down, use the Amazon GameLift server API <code>ProcessReady()</code> and specify one or more directory paths in <code>logParameters</code>.\
  \ For more information, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-api.html#gamelift-sdk-server-initialize\\\">Initialize the server process</a> in the <i>Amazon GameLift Developer Guide</i>. \"\n        }\n      ]\n    },\n    \"EC2InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceType\"\n        },\n        {\n          \"description\": \"The Amazon GameLift-supported Amazon EC2 instance type to use for all fleet instances. Instance type determines the computing resources that will be used to host your game servers, including CPU, memory, storage, and networking capacity. See <a href=\\\"http://aws.amazon.com/ec2/instance-types/\\\">Amazon Elastic Compute Cloud Instance Types</a> for detailed descriptions of Amazon EC2 instance types.\"\n        }\n      ]\n    },\n    \"EC2InboundPermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpPermissionsList\"\
  \n        },\n        {\n          \"description\": \"The allowed IP address ranges and port settings that allow inbound traffic to access game sessions on this fleet. If the fleet is hosting a custom game build, this property must be set before players can connect to game sessions. For Realtime Servers fleets, Amazon GameLift automatically sets TCP and UDP ranges. \"\n        }\n      ]\n    },\n    \"NewGameSessionProtectionPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtectionPolicy\"\n        },\n        {\n          \"description\": \"<p>The status of termination protection for active game sessions on the fleet. By default, this property is set to <code>NoProtection</code>. You can also set game session protection for an individual game session by calling <a href=\\\"gamelift/latest/apireference/API_UpdateGameSession.html\\\">UpdateGameSession</a>.</p> <ul> <li> <p> <b>NoProtection</b> - Game sessions can be terminated during active gameplay\
  \ as a result of a scale-down event. </p> </li> <li> <p> <b>FullProtection</b> - Game sessions in <code>ACTIVE</code> status cannot be terminated during a scale-down event.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"RuntimeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeConfiguration\"\n        },\n        {\n          \"description\": \"<p>Instructions for how to launch and maintain server processes on instances in the fleet. The runtime configuration defines one or more server process configurations, each identifying a build executable or Realtime script file and the number of processes of that type to run concurrently. </p> <note> <p>The <code>RuntimeConfiguration</code> parameter is required unless the fleet is being configured using the older parameters <code>ServerLaunchPath</code> and <code>ServerLaunchParameters</code>, which are still supported for backward compatibility.</p> </note>\"\n        }\n      ]\n    },\n\
  \    \"ResourceCreationLimitPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCreationLimitPolicy\"\n        },\n        {\n          \"description\": \"A policy that limits the number of game sessions that an individual player can create on instances in this fleet within a specified span of time.\"\n        }\n      ]\n    },\n    \"MetricGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricGroupList\"\n        },\n        {\n          \"description\": \"The name of an Amazon Web Services CloudWatch metric group to add this fleet to. A metric group is used to aggregate the metrics for multiple fleets. You can specify an existing metric group name or set a new name to create a new metric group. A fleet can be included in only one metric group at a time. \"\n        }\n      ]\n    },\n    \"PeerVpcAwsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\
  \n        },\n        {\n          \"description\": \"Used when peering your Amazon GameLift fleet with a VPC, the unique identifier for the Amazon Web Services account that owns the VPC. You can find your account ID in the Amazon Web Services Management Console under account settings. \"\n        }\n      ]\n    },\n    \"PeerVpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a VPC with resources to be accessed by your Amazon GameLift fleet. The VPC must be in the same Region as your fleet. To look up a VPC ID, use the <a href=\\\"https://console.aws.amazon.com/vpc/\\\">VPC Dashboard</a> in the Amazon Web Services Management Console. Learn more about VPC peering in <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/vpc-peering.html\\\">VPC Peering with Amazon GameLift Fleets</a>.\"\n        }\n      ]\n    },\n    \"FleetType\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetType\"\n        },\n        {\n          \"description\": \"Indicates whether to use On-Demand or Spot instances for this fleet. By default, this property is set to <code>ON_DEMAND</code>. Learn more about when to use <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-ec2-instances.html#gamelift-ec2-instances-spot\\\"> On-Demand versus Spot Instances</a>. This property cannot be changed after the fleet is created.\"\n        }\n      ]\n    },\n    \"InstanceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A unique identifier for an IAM role that manages access to your Amazon Web Services services. With an instance role ARN set, any application that runs on an instance in this fleet can assume the role, including install scripts, server processes, and daemons (background\
  \ processes). Create a role or look up a role's ARN by using the <a href=\\\"https://console.aws.amazon.com/iam/\\\">IAM dashboard</a> in the Amazon Web Services Management Console. Learn more about using on-box credentials for your game servers at <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/gamelift-sdk-server-resources.html\\\"> Access external resources from a game server</a>. This property cannot be changed after the fleet is created.\"\n        }\n      ]\n    },\n    \"CertificateConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateConfiguration\"\n        },\n        {\n          \"description\": \"<p>Prompts Amazon GameLift to generate a TLS/SSL certificate for the fleet. Amazon GameLift uses the certificates to encrypt traffic between game clients and the game servers running on Amazon GameLift. By default, the <code>CertificateConfiguration</code> is <code>DISABLED</code>. You can't change this property\
  \ after you create the fleet. </p> <p>Certificate Manager (ACM) certificates expire after 13 months. Certificate expiration can cause fleets to fail, preventing players from connecting to instances in the fleet. We recommend you replace fleets before 13 months, consider using fleet aliases for a smooth transition.</p> <note> <p>ACM isn't available in all Amazon Web Services regions. A fleet creation request with certificate generation enabled in an unsupported Region, fails with a 4xx error. For more information about the supported Regions, see <a href=\\\"https://docs.aws.amazon.com/acm/latest/userguide/acm-regions.html\\\">Supported Regions</a> in the <i>Certificate Manager User Guide</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"Locations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationConfigurationList\"\n        },\n        {\n          \"description\": \"<p>A set of remote locations to deploy additional instances to and manage as part\
  \ of the fleet. This parameter can only be used when creating fleets in Amazon Web Services Regions that support multiple locations. You can add any Amazon GameLift-supported Amazon Web Services Region as a remote location, in the form of an Amazon Web Services Region code such as <code>us-west-2</code>. To create a fleet with instances in the home Region only, don't use this parameter. </p> <p>To use this parameter, Amazon GameLift requires you to use your home location in the request.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of labels to assign to the new fleet resource. Tags are developer-defined key-value pairs. Tagging Amazon Web Services resources are useful for resource management, access management and cost allocation. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\"> Tagging\
  \ Amazon Web Services Resources</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    },\n    \"ComputeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n        },\n        {\n          \"description\": \"The type of compute resource used to host your game servers. You can use your own compute resources with Amazon GameLift Anywhere or use Amazon EC2 instances with managed Amazon GameLift. By default, this property is set to <code>EC2</code>.\"\n        }\n      ]\n    },\n    \"AnywhereConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnywhereConfiguration\"\n        },\n        {\n          \"description\": \"Amazon GameLift Anywhere configuration options.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateFleetInput
---
