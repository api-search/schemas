---
description: Placeholder documentation for BatchUpdateScheduleResponse
layout: schema
name: BatchUpdateScheduleResponse
properties_list:
- description: ''
  name: Creates
  type: object
- description: ''
  name: Deletes
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-update-schedule-response-schema.json
slug: medialive-api-batch-update-schedule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-update-schedule-response-schema.json\",\n  \"title\": \"BatchUpdateScheduleResponse\",\n  \"description\": \"Placeholder documentation for BatchUpdateScheduleResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Creates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchScheduleActionCreateResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creates\"\n          },\n          \"description\": \"Schedule actions created in the schedule.\"\n        }\n      ]\n    },\n    \"Deletes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchScheduleActionDeleteResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deletes\"\n          },\n          \"description\":\
  \ \"Schedule actions deleted from the schedule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-update-schedule-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BatchUpdateScheduleResponse
---
