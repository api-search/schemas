---
description: A list of schedule actions to delete.
layout: schema
name: BatchScheduleActionDeleteRequest
properties_list:
- description: ''
  name: ActionNames
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-schedule-action-delete-request-schema.json
slug: medialive-api-batch-schedule-action-delete-request
source_filename: medialive-api-batch-schedule-action-delete-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-schedule-action-delete-request-schema.json\",\n  \"title\": \"BatchScheduleActionDeleteRequest\",\n  \"description\": \"A list of schedule actions to delete.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"actionNames\"\n          },\n          \"description\": \"A list of schedule actions to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ActionNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-schedule-action-delete-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BatchScheduleActionDeleteRequest
---
