---
description: PublishStateMachineVersionInput schema from Amazon Step Functions API
layout: schema
name: PublishStateMachineVersionInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-publish-state-machine-version-input-schema.json
slug: amazon-step-functions-publish-state-machine-version-input
source_filename: amazon-step-functions-publish-state-machine-version-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-publish-state-machine-version-input-schema.json\",\n  \"title\": \"PublishStateMachineVersionInput\",\n  \"description\": \"PublishStateMachineVersionInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the state machine.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"<p>Only publish the state machine version if the current state machine's revision ID matches the specified ID.</p> <p>Use this option\
  \ to avoid publishing a version if the state machine changed since you last updated it. If the specified revision ID doesn't match the state machine's current revision ID, the API returns <code>ConflictException</code>.</p> <note> <p>To specify an initial revision ID for a state machine with no revision ID assigned, specify the string <code>INITIAL</code> for the <code>revisionId</code> parameter. For example, you can specify a <code>revisionID</code> of <code>INITIAL</code> when you create a state machine using the <a>CreateStateMachine</a> API action.</p> </note>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionDescription\"\n        },\n        {\n          \"description\": \"An optional description of the state machine version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-publish-state-machine-version-input-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: PublishStateMachineVersionInput
---
