---
description: Contains information on a single schedule action.
layout: schema
name: ScheduleAction
properties_list:
- description: ''
  name: ActionName
  type: object
- description: ''
  name: ScheduleActionSettings
  type: object
- description: ''
  name: ScheduleActionStartSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-schedule-action-schema.json
slug: medialive-api-schedule-action
source_filename: medialive-api-schedule-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-schedule-action-schema.json\",\n  \"title\": \"ScheduleAction\",\n  \"description\": \"Contains information on a single schedule action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"actionName\"\n          },\n          \"description\": \"The name of the action, must be unique within the schedule. This name provides the main reference to an action once it is added to the schedule. A name is unique if it is no longer in the schedule. The schedule is automatically cleaned up to remove actions with a start time of more than 1 hour ago (approximately) so at that point a name can be reused.\"\n        }\n      ]\n\
  \    },\n    \"ScheduleActionSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleActionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scheduleActionSettings\"\n          },\n          \"description\": \"Settings for this schedule action.\"\n        }\n      ]\n    },\n    \"ScheduleActionStartSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleActionStartSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scheduleActionStartSettings\"\n          },\n          \"description\": \"The time for the action to start in the channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ActionName\",\n    \"ScheduleActionStartSettings\",\n    \"ScheduleActionSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-schedule-action-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ScheduleAction
---
