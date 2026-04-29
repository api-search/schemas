---
description: The maintenance setting of a flow
layout: schema
name: Maintenance
properties_list:
- description: ''
  name: MaintenanceDay
  type: object
- description: ''
  name: MaintenanceDeadline
  type: object
- description: ''
  name: MaintenanceScheduledDate
  type: object
- description: ''
  name: MaintenanceStartHour
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-maintenance-schema.json
slug: mediaconnect-api-maintenance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-maintenance-schema.json\",\n  \"title\": \"Maintenance\",\n  \"description\": \"The maintenance setting of a flow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaintenanceDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceDay\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceDay\"\n          },\n          \"description\": \"A day of a week when the maintenance will happen. Use Monday/Tuesday/Wednesday/Thursday/Friday/Saturday/Sunday.\"\n        }\n      ]\n    },\n    \"MaintenanceDeadline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceDeadline\"\n          },\n          \"\
  description\": \"The Maintenance has to be performed before this deadline in ISO UTC format. Example: 2021-01-30T08:30:00Z.\"\n        }\n      ]\n    },\n    \"MaintenanceScheduledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceScheduledDate\"\n          },\n          \"description\": \"A scheduled date in ISO UTC format when the maintenance will happen. Use YYYY-MM-DD format. Example: 2021-01-30.\"\n        }\n      ]\n    },\n    \"MaintenanceStartHour\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceStartHour\"\n          },\n          \"description\": \"UTC time when the maintenance will happen. Use 24-hour HH:MM format. Minutes must be 00. Example: 13:00. The default value is 02:00.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-maintenance-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Maintenance
---
