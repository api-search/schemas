---
description: Represents information about the state of transitions between one stage and another stage.
layout: schema
name: TransitionState
properties_list:
- description: ''
  name: enabled
  type: object
- description: ''
  name: lastChangedBy
  type: object
- description: ''
  name: lastChangedAt
  type: object
- description: ''
  name: disabledReason
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-transition-state-schema.json
slug: amazon-codepipeline-transition-state
source_filename: amazon-codepipeline-transition-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-transition-state-schema.json\",\n  \"title\": \"TransitionState\",\n  \"description\": \"Represents information about the state of transitions between one stage and another stage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Enabled\"\n        },\n        {\n          \"description\": \"Whether the transition between stages is enabled (true) or disabled (false).\"\n        }\n      ]\n    },\n    \"lastChangedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastChangedBy\"\n        },\n        {\n          \"description\": \"The ID of the user who last changed the transition state.\"\n        }\n      ]\n    },\n    \"lastChangedAt\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/LastChangedAt\"\n        },\n        {\n          \"description\": \"The timestamp when the transition state was last changed.\"\n        }\n      ]\n    },\n    \"disabledReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisabledReason\"\n        },\n        {\n          \"description\": \"The user-specified reason why the transition between two stages of a pipeline was disabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-transition-state-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: TransitionState
---
