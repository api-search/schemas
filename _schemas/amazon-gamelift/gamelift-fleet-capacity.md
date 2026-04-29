---
description: <p>Current resource capacity settings in a specified fleet or location. The location value might refer to a fleet's remote location or its home Region. </p> <p> <b>Related actions</b> </p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribeFleetCapacity.html">DescribeFleetCapacity</a> | <a href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribeFleetLocationCapacity.html">DescribeFleetLocationCapacity</a> | <a href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_UpdateFleetCapacity.html">UpdateFleetCapacity</a> </p>
layout: schema
name: FleetCapacity
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: InstanceCounts
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-fleet-capacity-schema.json
slug: gamelift-fleet-capacity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-fleet-capacity-schema.json\",\n  \"title\": \"FleetCapacity\",\n  \"description\": \"<p>Current resource capacity settings in a specified fleet or location. The location value might refer to a fleet's remote location or its home Region. </p> <p> <b>Related actions</b> </p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribeFleetCapacity.html\\\">DescribeFleetCapacity</a> | <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_DescribeFleetLocationCapacity.html\\\">DescribeFleetLocationCapacity</a> | <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_UpdateFleetCapacity.html\\\">UpdateFleetCapacity</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet associated with the location.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift fleet resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceType\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instance type that is used for all instances in a fleet. The instance type determines the computing resources\
  \ in use, including CPU, memory, storage, and networking capacity. See <a href=\\\"http://aws.amazon.com/ec2/instance-types/\\\">Amazon Elastic Compute Cloud Instance Types</a> for detailed descriptions.\"\n        }\n      ]\n    },\n    \"InstanceCounts\": {\n      \"$ref\": \"#/components/schemas/EC2InstanceCounts\"\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The fleet location for the instance count information, expressed as an Amazon Web Services Region code, such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-fleet-capacity-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: FleetCapacity
---
