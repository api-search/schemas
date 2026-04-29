---
description: DescribeFleetLocationAttributesInput schema from Amazon GameLift API
layout: schema
name: DescribeFleetLocationAttributesInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: Locations
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-fleet-location-attributes-input-schema.json
slug: gamelift-describe-fleet-location-attributes-input
source_filename: gamelift-describe-fleet-location-attributes-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-location-attributes-input-schema.json\",\n  \"title\": \"DescribeFleetLocationAttributesInput\",\n  \"description\": \"DescribeFleetLocationAttributesInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to retrieve remote locations for. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"Locations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationList\"\n        },\n        {\n          \"description\": \"A list of fleet locations to retrieve information for. Specify locations in the\
  \ form of an Amazon Web Services Region code, such as <code>us-west-2</code>.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages. This limit is not currently enforced.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-location-attributes-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeFleetLocationAttributesInput
---
