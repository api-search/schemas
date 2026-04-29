---
description: NotifyApplicationStateRequest schema from Amazon Migration Hub API
layout: schema
name: NotifyApplicationStateRequest
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: UpdateDateTime
  type: object
- description: ''
  name: DryRun
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-notify-application-state-request-schema.json
slug: migration-hub-api-notify-application-state-request
source_filename: migration-hub-api-notify-application-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-notify-application-state-request-schema.json\",\n  \"title\": \"NotifyApplicationStateRequest\",\n  \"description\": \"NotifyApplicationStateRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationId\"\n        },\n        {\n          \"description\": \"The configurationId in Application Discovery Service that uniquely identifies the grouped application.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationStatus\"\n        },\n        {\n          \"description\": \"Status of the application - Not Started, In-Progress, Complete.\"\n        }\n      ]\n\
  \    },\n    \"UpdateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the application state changed.\"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRun\"\n        },\n        {\n          \"description\": \"Optional boolean flag to indicate whether any effect should take place. Used to test if the caller has permission to make the call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationId\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-notify-application-state-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NotifyApplicationStateRequest
---
