---
description: The parameters for using a Step Functions state machine as a target.
layout: schema
name: PipeTargetStateMachineParameters
properties_list:
- description: ''
  name: InvocationType
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-state-machine-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-state-machine-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-state-machine-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-state-machine-parameters-schema.json\",\n  \"title\": \"PipeTargetStateMachineParameters\",\n  \"description\": \"The parameters for using a Step Functions state machine as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvocationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetInvocationType\"\n        },\n        {\n          \"description\": \"Specify whether to wait for the state machine to finish or not.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-state-machine-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetStateMachineParameters
---
