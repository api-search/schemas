---
description: Information about a deployment lifecycle event.
layout: schema
name: LifecycleEvent
properties_list:
- description: ''
  name: lifecycleEventName
  type: object
- description: ''
  name: diagnostics
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-lifecycle-event-schema.json
slug: amazon-codedeploy-lifecycle-event
source_filename: amazon-codedeploy-lifecycle-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-lifecycle-event-schema.json\",\n  \"title\": \"LifecycleEvent\",\n  \"description\": \"Information about a deployment lifecycle event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lifecycleEventName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventName\"\n        },\n        {\n          \"description\": \"The deployment lifecycle event name, such as <code>ApplicationStop</code>, <code>BeforeInstall</code>, <code>AfterInstall</code>, <code>ApplicationStart</code>, or <code>ValidateService</code>.\"\n        }\n      ]\n    },\n    \"diagnostics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Diagnostics\"\n        },\n        {\n          \"description\": \"Diagnostic information about the deployment\
  \ lifecycle event.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when the deployment lifecycle event started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates when the deployment lifecycle event ended.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleEventStatus\"\n        },\n        {\n          \"description\": \"<p>The deployment lifecycle event status:</p> <ul> <li> <p>Pending: The deployment lifecycle event is pending.</p> </li> <li> <p>InProgress: The deployment lifecycle event is in progress.</p> </li> <li> <p>Succeeded: The deployment lifecycle event ran successfully.</p>\
  \ </li> <li> <p>Failed: The deployment lifecycle event has failed.</p> </li> <li> <p>Skipped: The deployment lifecycle event has been skipped.</p> </li> <li> <p>Unknown: The deployment lifecycle event is unknown.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-lifecycle-event-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: LifecycleEvent
---
