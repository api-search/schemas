---
description: An action performed by a direct agent and indirect participants upon a direct object. Optionally happens at a location.
layout: schema
name: Schema.org Action
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the action.
  name: name
  type: string
- description: A description of the action.
  name: description
  type: string
- description: URL associated with the action.
  name: url
  type: string
- description: Indicates the current disposition of the Action.
  name: actionStatus
  type: string
- description: The direct performer or driver of the action.
  name: agent
  type: object
- description: The object upon which the action is carried out.
  name: object
  type: object
- description: The result produced in the action.
  name: result
  type: object
- description: Indicates a target EntryPoint for an Action.
  name: target
  type: object
- description: The object that helped the agent perform the action.
  name: instrument
  type: object
- description: Other co-agents that participated in the action indirectly.
  name: participant
  type: object
- description: The location of the action.
  name: location
  type: object
- description: The startTime of something.
  name: startTime
  type: string
- description: The endTime of something.
  name: endTime
  type: string
- description: For failed actions, more information on the cause of the failure.
  name: error
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-action-schema.json
slug: schema-org-action
source_filename: schema-org-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/action.json\",\n  \"title\": \"Schema.org Action\",\n  \"description\": \"An action performed by a direct agent and indirect participants upon a direct object. Optionally happens at a location.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Action\", \"AchieveAction\", \"AssessAction\", \"ConsumeAction\", \"ControlAction\", \"CreateAction\", \"FindAction\", \"InteractAction\", \"MoveAction\", \"OrganizeAction\", \"PlayAction\", \"SearchAction\", \"SeekToAction\", \"SolveMathAction\", \"TradeAction\", \"TransferAction\", \"UpdateAction\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The name of the action.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the action.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL associated with the action.\"\n    },\n    \"actionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"ActiveActionStatus\", \"CompletedActionStatus\", \"FailedActionStatus\", \"PotentialActionStatus\"],\n      \"description\": \"Indicates the current disposition of the Action.\"\n    },\n    \"agent\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The direct performer or driver of the action.\"\n    },\n    \"object\": {\n      \"type\": \"object\",\n      \"description\": \"The object upon which the action is carried out.\",\n      \"properties\"\
  : {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"description\": \"The result produced in the action.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"target\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"#/$defs/EntryPoint\" }\n      ],\n      \"description\": \"Indicates a target EntryPoint for an Action.\"\n    },\n    \"instrument\": {\n      \"type\": \"object\",\n      \"description\": \"The object that helped the agent perform the action.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"participant\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\"\
  \ }\n      ],\n      \"description\": \"Other co-agents that participated in the action indirectly.\"\n    },\n    \"location\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-place-schema.json\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"The location of the action.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The startTime of something.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The endTime of something.\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"For failed actions, more information on the cause of the failure.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" }\n      }\n    },\n\
  \    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"EntryPoint\": {\n      \"type\": \"object\",\n      \"description\": \"An entry point for a URL-addressable action.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"EntryPoint\" },\n        \"urlTemplate\": { \"type\": \"string\", \"description\": \"A URL template for the action.\" },\n        \"httpMethod\": { \"type\": \"string\", \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"], \"description\": \"An HTTP method.\" },\n        \"contentType\": { \"type\": \"string\", \"description\": \"The supported content type(s).\" },\n        \"encodingType\": { \"type\": \"string\", \"description\": \"The supported\
  \ encoding type(s).\" },\n        \"actionPlatform\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ],\n          \"description\": \"The high level platform(s) where the Action can be performed for the given URL.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-action-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Action
---
