---
description: Contains details about an activity timeout that occurred during an execution.
layout: schema
name: ActivityTimedOutEventDetails
properties_list:
- description: ''
  name: error
  type: object
- description: ''
  name: cause
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-activity-timed-out-event-details-schema.json
slug: amazon-step-functions-activity-timed-out-event-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-activity-timed-out-event-details-schema.json\",\n  \"title\": \"ActivityTimedOutEventDetails\",\n  \"description\": \"Contains details about an activity timeout that occurred during an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveError\"\n        },\n        {\n          \"description\": \"The error code of the failure.\"\n        }\n      ]\n    },\n    \"cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveCause\"\n        },\n        {\n          \"description\": \"A more detailed explanation of the cause of the timeout.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-activity-timed-out-event-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: ActivityTimedOutEventDetails
---
