---
description: Settings for the action to deactivate the image in a specific layer.
layout: schema
name: StaticImageDeactivateScheduleActionSettings
properties_list:
- description: ''
  name: FadeOut
  type: object
- description: ''
  name: Layer
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-static-image-deactivate-schedule-action-settings-schema.json
slug: medialive-api-static-image-deactivate-schedule-action-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-static-image-deactivate-schedule-action-settings-schema.json\",\n  \"title\": \"StaticImageDeactivateScheduleActionSettings\",\n  \"description\": \"Settings for the action to deactivate the image in a specific layer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FadeOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fadeOut\"\n          },\n          \"description\": \"The time in milliseconds for the image to fade out. Default is 0 (no fade-out).\"\n        }\n      ]\n    },\n    \"Layer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max7\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"layer\"\
  \n          },\n          \"description\": \"The image overlay layer to deactivate, 0 to 7. Default is 0.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-static-image-deactivate-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StaticImageDeactivateScheduleActionSettings
---
