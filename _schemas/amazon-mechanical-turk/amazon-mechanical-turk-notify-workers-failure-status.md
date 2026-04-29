---
description: When MTurk encounters an issue with notifying the Workers you specified, it returns back this object with failure details.
layout: schema
name: NotifyWorkersFailureStatus
properties_list:
- description: ''
  name: NotifyWorkersFailureCode
  type: object
- description: ''
  name: NotifyWorkersFailureMessage
  type: object
- description: ''
  name: WorkerId
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-notify-workers-failure-status-schema.json
slug: amazon-mechanical-turk-notify-workers-failure-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-notify-workers-failure-status-schema.json\",\n  \"title\": \"NotifyWorkersFailureStatus\",\n  \"description\": \" When MTurk encounters an issue with notifying the Workers you specified, it returns back this object with failure details. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotifyWorkersFailureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyWorkersFailureCode\"\n        },\n        {\n          \"description\": \" Encoded value for the failure type. \"\n        }\n      ]\n    },\n    \"NotifyWorkersFailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A message detailing the reason the Worker could not be notified.\
  \ \"\n        }\n      ]\n    },\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \" The ID of the Worker.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-notify-workers-failure-status-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: NotifyWorkersFailureStatus
---
