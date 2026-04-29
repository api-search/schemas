---
description: GetIncidentRecordOutput schema
layout: schema
name: GetIncidentRecordOutput
properties_list:
- description: ''
  name: incidentRecord
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-get-incident-record-output-schema.json
slug: incident-manager-get-incident-record-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-incident-record-output-schema.json\",\n  \"title\": \"GetIncidentRecordOutput\",\n  \"description\": \"GetIncidentRecordOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incidentRecord\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentRecord\"\n        },\n        {\n          \"description\": \"Details the structure of the incident record.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentRecord\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-incident-record-output-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: GetIncidentRecordOutput
---
