---
description: CreateAliasInput schema from Amazon GameLift API
layout: schema
name: CreateAliasInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: RoutingStrategy
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-alias-input-schema.json
slug: gamelift-create-alias-input
source_filename: gamelift-create-alias-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-alias-input-schema.json\",\n  \"title\": \"CreateAliasInput\",\n  \"description\": \"CreateAliasInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonBlankAndLengthConstraintString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with an alias. Alias names do not need to be unique.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A human-readable description of the alias.\"\n        }\n      ]\n    },\n    \"RoutingStrategy\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/RoutingStrategy\"\n        },\n        {\n          \"description\": \"The routing configuration, including routing type and fleet target, for the alias. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of labels to assign to the new alias resource. Tags are developer-defined key-value pairs. Tagging Amazon Web Services resources are useful for resource management, access management and cost allocation. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\"> Tagging Amazon Web Services Resources</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RoutingStrategy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-alias-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateAliasInput
---
