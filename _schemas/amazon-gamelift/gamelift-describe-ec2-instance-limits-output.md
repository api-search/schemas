---
description: DescribeEC2InstanceLimitsOutput schema from Amazon GameLift API
layout: schema
name: DescribeEC2InstanceLimitsOutput
properties_list:
- description: ''
  name: EC2InstanceLimits
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-ec2-instance-limits-output-schema.json
slug: gamelift-describe-ec2-instance-limits-output
source_filename: gamelift-describe-ec2-instance-limits-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-ec2-instance-limits-output-schema.json\",\n  \"title\": \"DescribeEC2InstanceLimitsOutput\",\n  \"description\": \"DescribeEC2InstanceLimitsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EC2InstanceLimits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceLimitList\"\n        },\n        {\n          \"description\": \"The maximum number of instances for the specified instance type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-ec2-instance-limits-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeEC2InstanceLimitsOutput
---
