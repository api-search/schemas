---
description: Details about the PagerDuty service where the response plan creates an incident.
layout: schema
name: PagerDutyIncidentConfiguration
properties_list:
- description: ''
  name: serviceId
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-pager-duty-incident-configuration-schema.json
slug: incident-manager-pager-duty-incident-configuration
source_filename: incident-manager-pager-duty-incident-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-pager-duty-incident-configuration-schema.json\",\n  \"title\": \"PagerDutyIncidentConfiguration\",\n  \"description\": \"Details about the PagerDuty service where the response plan creates an incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyIncidentConfigurationServiceIdString\"\n        },\n        {\n          \"description\": \"The ID of the PagerDuty service that the response plan associates with an incident when it launches.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-pager-duty-incident-configuration-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: PagerDutyIncidentConfiguration
---
