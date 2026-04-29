---
description: NotifyWorkersRequest schema from Amazon Mechanical Turk API
layout: schema
name: NotifyWorkersRequest
properties_list:
- description: ''
  name: Subject
  type: object
- description: ''
  name: MessageText
  type: object
- description: ''
  name: WorkerIds
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-notify-workers-request-schema.json
slug: amazon-mechanical-turk-notify-workers-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-notify-workers-request-schema.json\",\n  \"title\": \"NotifyWorkersRequest\",\n  \"description\": \"NotifyWorkersRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Subject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The subject line of the email message to send. Can include up to 200 characters.\"\n        }\n      ]\n    },\n    \"MessageText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The text of the email message to send. Can include up to 4,096 characters\"\n        }\n      ]\n    },\n    \"WorkerIds\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/CustomerIdList\"\n        },\n        {\n          \"description\": \"A list of Worker IDs you wish to notify. You can notify upto 100 Workers at a time.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Subject\",\n    \"MessageText\",\n    \"WorkerIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-notify-workers-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: NotifyWorkersRequest
---
