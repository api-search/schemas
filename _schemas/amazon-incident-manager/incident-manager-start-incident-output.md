---
description: StartIncidentOutput schema
layout: schema
name: StartIncidentOutput
properties_list:
- description: ''
  name: incidentRecordArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-start-incident-output-schema.json
slug: incident-manager-start-incident-output
source_filename: incident-manager-start-incident-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-start-incident-output-schema.json\",\n  \"title\": \"StartIncidentOutput\",\n  \"description\": \"StartIncidentOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the newly created incident record.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-start-incident-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: StartIncidentOutput
---
