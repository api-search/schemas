---
description: Settings to specify the rendering of motion graphics into the video stream.
layout: schema
name: MotionGraphicsActivateScheduleActionSettings
properties_list:
- description: ''
  name: Duration
  type: object
- description: ''
  name: PasswordParam
  type: object
- description: ''
  name: Url
  type: object
- description: ''
  name: Username
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-motion-graphics-activate-schedule-action-settings-schema.json
slug: medialive-api-motion-graphics-activate-schedule-action-settings
source_filename: medialive-api-motion-graphics-activate-schedule-action-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-motion-graphics-activate-schedule-action-settings-schema.json\",\n  \"title\": \"MotionGraphicsActivateScheduleActionSettings\",\n  \"description\": \"Settings to specify the rendering of motion graphics into the video stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__longMin0Max86400000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"duration\"\n          },\n          \"description\": \"Duration (in milliseconds) that motion graphics should render on to the video stream. Leaving out this property or setting to 0 will result in rendering continuing until a deactivate action is processed.\"\n        }\n      ]\n    },\n    \"PasswordParam\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passwordParam\"\n          },\n          \"description\": \"Key used to extract the password from EC2 Parameter store\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"URI of the HTML5 content to be rendered into the live stream.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-motion-graphics-activate-schedule-action-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MotionGraphicsActivateScheduleActionSettings
---
