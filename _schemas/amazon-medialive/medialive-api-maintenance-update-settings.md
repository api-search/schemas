---
description: Placeholder documentation for MaintenanceUpdateSettings
layout: schema
name: MaintenanceUpdateSettings
properties_list:
- description: ''
  name: MaintenanceDay
  type: object
- description: ''
  name: MaintenanceScheduledDate
  type: object
- description: ''
  name: MaintenanceStartTime
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-maintenance-update-settings-schema.json
slug: medialive-api-maintenance-update-settings
source_filename: medialive-api-maintenance-update-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-maintenance-update-settings-schema.json\",\n  \"title\": \"MaintenanceUpdateSettings\",\n  \"description\": \"Placeholder documentation for MaintenanceUpdateSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaintenanceDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceDay\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceDay\"\n          },\n          \"description\": \"Choose one day of the week for maintenance. The chosen day is used for all future maintenance windows.\"\n        }\n      ]\n    },\n    \"MaintenanceScheduledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceScheduledDate\"\
  \n          },\n          \"description\": \"Choose a specific date for maintenance to occur. The chosen date is used for the next maintenance window only.\"\n        }\n      ]\n    },\n    \"MaintenanceStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern010920300\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceStartTime\"\n          },\n          \"description\": \"Choose the hour that maintenance will start. The chosen time is used for all future maintenance windows.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-maintenance-update-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MaintenanceUpdateSettings
---
