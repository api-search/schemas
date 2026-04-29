---
description: ListStateMachineVersionsOutput schema from Amazon Step Functions API
layout: schema
name: ListStateMachineVersionsOutput
properties_list:
- description: ''
  name: stateMachineVersions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-list-state-machine-versions-output-schema.json
slug: amazon-step-functions-list-state-machine-versions-output
source_filename: amazon-step-functions-list-state-machine-versions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-list-state-machine-versions-output-schema.json\",\n  \"title\": \"ListStateMachineVersionsOutput\",\n  \"description\": \"ListStateMachineVersionsOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateMachineVersionList\"\n        },\n        {\n          \"description\": \"Versions for the state machine.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"If <code>nextToken</code> is returned, there are more results available. The value of <code>nextToken</code> is a unique pagination token\
  \ for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return an <i>HTTP 400 InvalidToken</i> error.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"stateMachineVersions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-list-state-machine-versions-output-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: ListStateMachineVersionsOutput
---
