---
description: ListAliasesInput schema from Amazon GameLift API
layout: schema
name: ListAliasesInput
properties_list:
- description: ''
  name: RoutingStrategyType
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-list-aliases-input-schema.json
slug: gamelift-list-aliases-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-aliases-input-schema.json\",\n  \"title\": \"ListAliasesInput\",\n  \"description\": \"ListAliasesInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoutingStrategyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutingStrategyType\"\n        },\n        {\n          \"description\": \"<p>The routing type to filter results on. Use this parameter to retrieve only aliases with a certain routing type. To retrieve all aliases, leave this parameter empty.</p> <p>Possible routing types include the following:</p> <ul> <li> <p> <b>SIMPLE</b> -- The alias resolves to one specific fleet. Use this type when routing to active fleets.</p> </li> <li> <p> <b>TERMINAL</b> -- The alias does not resolve to a fleet but instead can\
  \ be used to display a message to the user. A terminal alias throws a TerminalRoutingStrategyException with the <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_RoutingStrategy.html\\\">RoutingStrategy</a> message embedded.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with an alias. Alias names do not need to be unique.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to return. Use this parameter with <code>NextToken</code> to get results as a set of sequential pages.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\
  \n        },\n        {\n          \"description\": \"A token that indicates the start of the next sequential page of results. Use the token that is returned with a previous call to this operation. To start at the beginning of the result set, do not specify a value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-list-aliases-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ListAliasesInput
---
