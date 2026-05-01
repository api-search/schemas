---
description: Information about third-party services integrated into a response plan.
layout: schema
name: Integration
properties_list:
- description: ''
  name: pagerDutyConfiguration
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-integration-schema.json
slug: incident-manager-integration
source_filename: incident-manager-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-integration-schema.json\",\n  \"title\": \"Integration\",\n  \"description\": \"Information about third-party services integrated into a response plan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pagerDutyConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyConfiguration\"\n        },\n        {\n          \"description\": \"Information about the PagerDuty service where the response plan creates an incident.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-integration-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: Integration
---
