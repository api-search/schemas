---
description: The information about the maintenance schedule.
layout: schema
name: MaintenanceSchedule
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: startTime
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-maintenance-schedule-schema.json
slug: amazon-mainframe-modernization-maintenance-schedule
source_filename: amazon-mainframe-modernization-maintenance-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-maintenance-schedule-schema.json\",\n  \"title\": \"MaintenanceSchedule\",\n  \"description\": \"The information about the maintenance schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the scheduled maintenance is to end.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the scheduled maintenance is to start.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-maintenance-schedule-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: MaintenanceSchedule
---
