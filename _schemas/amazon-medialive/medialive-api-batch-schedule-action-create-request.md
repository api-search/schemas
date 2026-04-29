---
description: A list of schedule actions to create (in a request) or that have been created (in a response).
layout: schema
name: BatchScheduleActionCreateRequest
properties_list:
- description: ''
  name: ScheduleActions
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-schedule-action-create-request-schema.json
slug: medialive-api-batch-schedule-action-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-schedule-action-create-request-schema.json\",\n  \"title\": \"BatchScheduleActionCreateRequest\",\n  \"description\": \"A list of schedule actions to create (in a request) or that have been created (in a response).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduleActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfScheduleAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scheduleActions\"\n          },\n          \"description\": \"A list of schedule actions to create.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduleActions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-schedule-action-create-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BatchScheduleActionCreateRequest
---
