---
description: Integrations schema
layout: schema
name: Integrations
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-integrations-schema.json
slug: incident-manager-integrations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-integrations-schema.json\",\n  \"title\": \"Integrations\",\n  \"description\": \"Integrations schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"pagerDutyConfiguration\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PagerDutyConfiguration\"\n          },\n          {\n            \"description\": \"Information about the PagerDuty service where the response plan creates an incident.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about third-party services integrated into a response plan.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-integrations-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: Integrations
---
