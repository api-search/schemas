---
description: List of actions to create and list of actions to delete.
layout: schema
name: BatchUpdateScheduleRequest
properties_list:
- description: ''
  name: Creates
  type: object
- description: ''
  name: Deletes
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-update-schedule-request-schema.json
slug: medialive-api-batch-update-schedule-request
source_filename: medialive-api-batch-update-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-update-schedule-request-schema.json\",\n  \"title\": \"BatchUpdateScheduleRequest\",\n  \"description\": \"List of actions to create and list of actions to delete.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Creates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchScheduleActionCreateRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creates\"\n          },\n          \"description\": \"Schedule actions to create in the schedule.\"\n        }\n      ]\n    },\n    \"Deletes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchScheduleActionDeleteRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deletes\"\n          },\n          \"description\"\
  : \"Schedule actions to delete from the schedule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-update-schedule-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BatchUpdateScheduleRequest
---
