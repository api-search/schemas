---
description: <p>Set of rule statements, used with FlexMatch, that determine how to build your player matches. Each rule set describes a type of group to be created and defines the parameters for acceptable player matches.</p> <p>A rule set may define the following elements for a match. For detailed information and examples showing how to construct a rule set, see <a href="https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-rulesets.html">Build a FlexMatch rule set</a>. </p> <ul> <li> <p>Teams -- Required. A rule set must define one or multiple teams for the match and set minimum and maximum team sizes. For example, a rule set might describe a 4x4 match that requires all eight slots to be filled. </p> </li> <li> <p>Player attributes -- Optional. These attributes specify a set of player characteristics to evaluate when looking for a match. Matchmaking requests that use a rule set with player attributes must provide the corresponding attribute values. For example, an attribute
  might specify a player's skill or level.</p> </li> <li> <p>Rules -- Optional. Rules define how to evaluate potential players for a match based on player attributes. A rule might specify minimum requirements for individual players, teams, or entire matches. For example, a rule might require each player to meet a certain skill level, each team to have at least one player in a certain role, or the match to have a minimum average skill level. or may describe an entire group--such as all teams must be evenly matched or have at least one player in a certain role. </p> </li> <li> <p>Expansions -- Optional. Expansions allow you to relax the rules after a period of time when no acceptable matches are found. This feature lets you balance getting players into games in a reasonable amount of time instead of making them wait indefinitely for the best possible match. For example, you might use an expansion to increase the maximum skill variance between players after 30 seconds.</p> </li> </ul>
layout: schema
name: MatchmakingRuleSet
properties_list:
- description: ''
  name: RuleSetName
  type: object
- description: ''
  name: RuleSetArn
  type: object
- description: ''
  name: RuleSetBody
  type: object
- description: ''
  name: CreationTime
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-matchmaking-rule-set-schema.json
slug: gamelift-matchmaking-rule-set
source_filename: gamelift-matchmaking-rule-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matchmaking-rule-set-schema.json\",\n  \"title\": \"MatchmakingRuleSet\",\n  \"description\": \"<p>Set of rule statements, used with FlexMatch, that determine how to build your player matches. Each rule set describes a type of group to be created and defines the parameters for acceptable player matches.</p> <p>A rule set may define the following elements for a match. For detailed information and examples showing how to construct a rule set, see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/flexmatchguide/match-rulesets.html\\\">Build a FlexMatch rule set</a>. </p> <ul> <li> <p>Teams -- Required. A rule set must define one or multiple teams for the match and set minimum and maximum team sizes. For example, a rule set might describe a 4x4 match that requires all eight slots to be filled.\
  \ </p> </li> <li> <p>Player attributes -- Optional. These attributes specify a set of player characteristics to evaluate when looking for a match. Matchmaking requests that use a rule set with player attributes must provide the corresponding attribute values. For example, an attribute might specify a player's skill or level.</p> </li> <li> <p>Rules -- Optional. Rules define how to evaluate potential players for a match based on player attributes. A rule might specify minimum requirements for individual players, teams, or entire matches. For example, a rule might require each player to meet a certain skill level, each team to have at least one player in a certain role, or the match to have a minimum average skill level. or may describe an entire group--such as all teams must be evenly matched or have at least one player in a certain role. </p> </li> <li> <p>Expansions -- Optional. Expansions allow you to relax the rules after a period of time when no acceptable matches are found. This feature\
  \ lets you balance getting players into games in a reasonable amount of time instead of making them wait indefinitely for the best possible match. For example, you might use an expansion to increase the maximum skill variance between players after 30 seconds.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking rule set\"\n        }\n      ]\n    },\n    \"RuleSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingRuleSetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift matchmaking rule set resource and uniquely identifies it. ARNs are unique across all Regions.\
  \ Format is <code>arn:aws:gamelift:&lt;region&gt;::matchmakingruleset/&lt;ruleset name&gt;</code>. In a GameLift rule set ARN, the resource ID matches the <i>RuleSetName</i> value.\"\n        }\n      ]\n    },\n    \"RuleSetBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleSetBody\"\n        },\n        {\n          \"description\": \"A collection of matchmaking rules, formatted as a JSON string. Comments are not allowed in JSON, but most elements support a description field.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleSetBody\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-matchmaking-rule-set-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: MatchmakingRuleSet
---
