---
description: Settings for the action to set pause state of a channel.
layout: schema
name: PauseStateScheduleActionSettings
properties_list:
- description: ''
  name: Pipelines
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-pause-state-schedule-action-settings-schema.json
slug: medialive-api-pause-state-schedule-action-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-pause-state-schedule-action-settings-schema.json\",\n  \"title\": \"PauseStateScheduleActionSettings\",\n  \"description\": \"Settings for the action to set pause state of a channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pipelines\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfPipelinePauseStateSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelines\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-pause-state-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PauseStateScheduleActionSettings
---
