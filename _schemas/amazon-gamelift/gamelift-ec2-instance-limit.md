---
description: The Amazon GameLift service limits for an Amazon EC2 instance type and current utilization. Amazon GameLift allows Amazon Web Services accounts a maximum number of instances, per instance type, per Amazon Web Services Region or location, for use with Amazon GameLift. You can request an limit increase for your account by using the <b>Service limits</b> page in the Amazon GameLift console.
layout: schema
name: EC2InstanceLimit
properties_list:
- description: ''
  name: EC2InstanceType
  type: object
- description: ''
  name: CurrentInstances
  type: object
- description: ''
  name: InstanceLimit
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-ec2-instance-limit-schema.json
slug: gamelift-ec2-instance-limit
source_filename: gamelift-ec2-instance-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-ec2-instance-limit-schema.json\",\n  \"title\": \"EC2InstanceLimit\",\n  \"description\": \"The Amazon GameLift service limits for an Amazon EC2 instance type and current utilization. Amazon GameLift allows Amazon Web Services accounts a maximum number of instances, per instance type, per Amazon Web Services Region or location, for use with Amazon GameLift. You can request an limit increase for your account by using the <b>Service limits</b> page in the Amazon GameLift console.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EC2InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceType\"\n        },\n        {\n          \"description\": \"The name of an Amazon EC2 instance type. See <a href=\\\"http://aws.amazon.com/ec2/instance-types/\\\
  \">Amazon Elastic Compute Cloud Instance Types</a> for detailed descriptions. \"\n        }\n      ]\n    },\n    \"CurrentInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of instances for the specified type and location that are currently being used by the Amazon Web Services account. \"\n        }\n      ]\n    },\n    \"InstanceLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of instances that is allowed for the specified instance type and location.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"An Amazon Web Services Region code, such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-ec2-instance-limit-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: EC2InstanceLimit
---
