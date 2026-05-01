---
description: DescribeScalingPoliciesInput schema from Amazon GameLift API
layout: schema
name: DescribeScalingPoliciesInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: StatusFilter
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-scaling-policies-input-schema.json
slug: gamelift-describe-scaling-policies-input
source_filename: gamelift-describe-scaling-policies-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-scaling-policies-input-schema.json\",\n  \"title\": \"DescribeScalingPoliciesInput\",\n  \"description\": \"DescribeScalingPoliciesInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet for which to retrieve scaling policies. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"StatusFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingStatusType\"\n        },\n        {\n          \"description\": \"<p>Scaling policy status to filter results on. A scaling policy is only in force when in an\
  \ <code>ACTIVE</code> status.</p> <ul> <li> <p> <b>ACTIVE</b> -- The scaling policy is currently in force.</p> </li> <li> <p> <b>UPDATEREQUESTED</b> -- A request to update the scaling policy has been received.</p> </li> <li> <p> <b>UPDATING</b> -- A change is being made to the scaling policy.</p> </li> <li> <p> <b>DELETEREQUESTED</b> -- A request to delete the scaling policy has been received.</p> </li> <li> <p> <b>DELETING</b> -- The scaling policy is being deleted.</p> </li> <li> <p> <b>DELETED</b> -- The scaling policy has been deleted.</p> </li> <li> <p> <b>ERROR</b> -- An error occurred in creating the policy. It should be removed and recreated.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages.\"\
  \n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \" The fleet location. If you don't specify this value, the response contains the scaling policies of every location in the fleet. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-scaling-policies-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeScalingPoliciesInput
---
