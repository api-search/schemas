---
description: DescribeFleetAttributesInput schema from Amazon GameLift API
layout: schema
name: DescribeFleetAttributesInput
properties_list:
- description: ''
  name: FleetIds
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-fleet-attributes-input-schema.json
slug: gamelift-describe-fleet-attributes-input
source_filename: gamelift-describe-fleet-attributes-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-attributes-input-schema.json\",\n  \"title\": \"DescribeFleetAttributesInput\",\n  \"description\": \"DescribeFleetAttributesInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArnList\"\n        },\n        {\n          \"description\": \"A list of unique fleet identifiers to retrieve attributes for. You can use either the fleet ID or ARN value. To retrieve attributes for all current fleets, do not include this parameter. \"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results\
  \ to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages. This parameter is ignored when the request specifies one or a list of fleet IDs.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value. This parameter is ignored when the request specifies one or a list of fleet IDs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-attributes-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeFleetAttributesInput
---
