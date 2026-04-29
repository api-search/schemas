---
description: The scheduled maintenance for a runtime engine.
layout: schema
name: PendingMaintenance
properties_list:
- description: ''
  name: engineVersion
  type: object
- description: ''
  name: schedule
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-pending-maintenance-schema.json
slug: amazon-mainframe-modernization-pending-maintenance
source_filename: amazon-mainframe-modernization-pending-maintenance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-pending-maintenance-schema.json\",\n  \"title\": \"PendingMaintenance\",\n  \"description\": \"The scheduled maintenance for a runtime engine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"engineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The specific runtime engine that the maintenance schedule applies to.\"\n        }\n      ]\n    },\n    \"schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceSchedule\"\n        },\n        {\n          \"description\": \"The maintenance schedule for the runtime engine version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-pending-maintenance-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: PendingMaintenance
---
