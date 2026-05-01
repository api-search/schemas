---
description: RegisterComputeInput schema from Amazon GameLift API
layout: schema
name: RegisterComputeInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: ComputeName
  type: object
- description: ''
  name: CertificatePath
  type: object
- description: ''
  name: DnsName
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-register-compute-input-schema.json
slug: gamelift-register-compute-input
source_filename: gamelift-register-compute-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-register-compute-input-schema.json\",\n  \"title\": \"RegisterComputeInput\",\n  \"description\": \"RegisterComputeInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to register the compute to. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"ComputeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeName\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with the compute resource registered to your fleet.\"\n        }\n      ]\n    },\n    \"CertificatePath\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"The path to the TLS certificate on your compute resource. The path and certificate are not validated by Amazon GameLift.\"\n        }\n      ]\n    },\n    \"DnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsNameInput\"\n        },\n        {\n          \"description\": \"The DNS name of the compute resource. Amazon GameLift requires the DNS name or IP address to manage your compute resource.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the compute resource. Amazon GameLift requires the DNS name or IP address to manage your compute resource.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The name of the custom location you added to the fleet you are registering this compute resource to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"ComputeName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-register-compute-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: RegisterComputeInput
---
