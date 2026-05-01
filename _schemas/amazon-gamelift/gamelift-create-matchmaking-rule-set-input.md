---
description: CreateMatchmakingRuleSetInput schema from Amazon GameLift API
layout: schema
name: CreateMatchmakingRuleSetInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RuleSetBody
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-matchmaking-rule-set-input-schema.json
slug: gamelift-create-matchmaking-rule-set-input
source_filename: gamelift-create-matchmaking-rule-set-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-matchmaking-rule-set-input-schema.json\",\n  \"title\": \"CreateMatchmakingRuleSetInput\",\n  \"description\": \"CreateMatchmakingRuleSetInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdStringModel\"\n        },\n        {\n          \"description\": \"A unique identifier for the matchmaking rule set. A matchmaking configuration identifies the rule set it uses by this name value. Note that the rule set name is different from the optional <code>name</code> field in the rule set body.\"\n        }\n      ]\n    },\n    \"RuleSetBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleSetBody\"\n        },\n        {\n\
  \          \"description\": \"A collection of matchmaking rules, formatted as a JSON string. Comments are not allowed in JSON, but most elements support a description field.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of labels to assign to the new matchmaking rule set resource. Tags are developer-defined key-value pairs. Tagging Amazon Web Services resources are useful for resource management, access management and cost allocation. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\"> Tagging Amazon Web Services Resources</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RuleSetBody\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-matchmaking-rule-set-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateMatchmakingRuleSetInput
---
