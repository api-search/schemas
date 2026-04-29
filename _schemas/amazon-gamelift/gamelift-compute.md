---
description: Resources used to host your game servers. A compute resource can be managed Amazon GameLift Amazon EC2 instances or your own resources.
layout: schema
name: Compute
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: ComputeName
  type: object
- description: ''
  name: ComputeArn
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: DnsName
  type: object
- description: ''
  name: ComputeStatus
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: OperatingSystem
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: GameLiftServiceSdkEndpoint
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-compute-schema.json
slug: gamelift-compute
source_filename: gamelift-compute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-compute-schema.json\",\n  \"title\": \"Compute\",\n  \"description\": \"Resources used to host your game servers. A compute resource can be managed Amazon GameLift Amazon EC2 instances or your own resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that the compute is registered to.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet that the compute is registered to.\"\n        }\n      ]\n    },\n    \"ComputeName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeName\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with the compute resource registered to your fleet.\"\n        }\n      ]\n    },\n    \"ComputeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeArn\"\n        },\n        {\n          \"description\": \"The ARN that is assigned to the compute resource and uniquely identifies it. ARNs are unique across locations.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the compute resource. Amazon GameLift requires the DNS name or IP address to manage your compute resource.\"\n        }\n      ]\n    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsName\"\n    \
  \    },\n        {\n          \"description\": \"The DNS name of the compute resource. Amazon GameLift requires the DNS name or IP address to manage your compute resource.\"\n        }\n      ]\n    },\n    \"ComputeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeStatus\"\n        },\n        {\n          \"description\": \"Current status of the compute. A compute must have an <code>ACTIVE</code> status to host game sessions.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The name of the custom location you added to the fleet that this compute resource resides in.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this\
  \ data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"The type of operating system on your compute resource.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceType\"\n        },\n        {\n          \"description\": \"The compute type that the fleet uses. A fleet can use Anywhere compute resources that you own, or use managed Amazon EC2 instances.\"\n        }\n      ]\n    },\n    \"GameLiftServiceSdkEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GameLiftServiceSdkEndpointOutput\"\n        },\n        {\n          \"description\": \"The endpoint connection details of the Amazon GameLift\
  \ SDK endpoint that your game server connects to.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-compute-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: Compute
---
