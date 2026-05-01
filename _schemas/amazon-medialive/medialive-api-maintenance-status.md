---
description: Placeholder documentation for MaintenanceStatus
layout: schema
name: MaintenanceStatus
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
  name: MaintenanceStartTime
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-maintenance-status-schema.json
slug: medialive-api-maintenance-status
source_filename: medialive-api-maintenance-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-maintenance-status-schema.json\",\n  \"title\": \"MaintenanceStatus\",\n  \"description\": \"Placeholder documentation for MaintenanceStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaintenanceDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceDay\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceDay\"\n          },\n          \"description\": \"The currently selected maintenance day.\"\n        }\n      ]\n    },\n    \"MaintenanceDeadline\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceDeadline\"\n          },\n          \"description\": \"Maintenance is required by the displayed\
  \ date and time. Date and time is in ISO.\"\n        }\n      ]\n    },\n    \"MaintenanceScheduledDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceScheduledDate\"\n          },\n          \"description\": \"The currently scheduled maintenance date and time. Date and time is in ISO.\"\n        }\n      ]\n    },\n    \"MaintenanceStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceStartTime\"\n          },\n          \"description\": \"The currently selected maintenance start time. Time is in UTC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-maintenance-status-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MaintenanceStatus
---
