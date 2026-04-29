---
description: Create maintenance setting for a flow
layout: schema
name: AddMaintenance
properties_list:
- description: ''
  name: MaintenanceDay
  type: object
- description: ''
  name: MaintenanceStartHour
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-maintenance-schema.json
slug: mediaconnect-api-add-maintenance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-maintenance-schema.json\",\n  \"title\": \"AddMaintenance\",\n  \"description\": \"Create maintenance setting for a flow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaintenanceDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceDay\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceDay\"\n          },\n          \"description\": \"A day of a week when the maintenance will happen. Use Monday/Tuesday/Wednesday/Thursday/Friday/Saturday/Sunday.\"\n        }\n      ]\n    },\n    \"MaintenanceStartHour\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceStartHour\"\n          },\n\
  \          \"description\": \"UTC time when the maintenance will happen. Use 24-hour HH:MM format. Minutes must be 00. Example: 13:00. The default value is 02:00.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaintenanceDay\",\n    \"MaintenanceStartHour\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-maintenance-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddMaintenance
---
