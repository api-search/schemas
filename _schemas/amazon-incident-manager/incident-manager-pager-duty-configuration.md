---
description: Details about the PagerDuty configuration for a response plan.
layout: schema
name: PagerDutyConfiguration
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: pagerDutyIncidentConfiguration
  type: object
- description: ''
  name: secretId
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-pager-duty-configuration-schema.json
slug: incident-manager-pager-duty-configuration
source_filename: incident-manager-pager-duty-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-pager-duty-configuration-schema.json\",\n  \"title\": \"PagerDutyConfiguration\",\n  \"description\": \"Details about the PagerDuty configuration for a response plan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyConfigurationNameString\"\n        },\n        {\n          \"description\": \"The name of the PagerDuty configuration.\"\n        }\n      ]\n    },\n    \"pagerDutyIncidentConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyIncidentConfiguration\"\n        },\n        {\n          \"description\": \"Details about the PagerDuty service associated with the configuration.\"\n        }\n      ]\n    },\n    \"secretId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyConfigurationSecretIdString\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services Secrets Manager secret that stores your PagerDuty key, either a General Access REST API Key or User Token REST API Key, and other user credentials.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"pagerDutyIncidentConfiguration\",\n    \"secretId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-pager-duty-configuration-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: PagerDutyConfiguration
---
