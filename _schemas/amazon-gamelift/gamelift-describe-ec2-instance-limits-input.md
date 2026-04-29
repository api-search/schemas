---
description: DescribeEC2InstanceLimitsInput schema from Amazon GameLift API
layout: schema
name: DescribeEC2InstanceLimitsInput
properties_list:
- description: ''
  name: EC2InstanceType
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-ec2-instance-limits-input-schema.json
slug: gamelift-describe-ec2-instance-limits-input
source_filename: gamelift-describe-ec2-instance-limits-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-ec2-instance-limits-input-schema.json\",\n  \"title\": \"DescribeEC2InstanceLimitsInput\",\n  \"description\": \"DescribeEC2InstanceLimitsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EC2InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceType\"\n        },\n        {\n          \"description\": \"Name of an Amazon EC2 instance type that is supported in Amazon GameLift. A fleet instance type determines the computing resources of each instance in the fleet, including CPU, memory, storage, and networking capacity. Do not specify a value for this parameter to retrieve limits for all instance types.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The name of a remote location to request instance limits for, in the form of an Amazon Web Services Region code such as <code>us-west-2</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-ec2-instance-limits-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeEC2InstanceLimitsInput
---
