---
description: Details about the PagerDuty incident associated with an incident created by an Incident Manager response plan.
layout: schema
name: PagerDutyIncidentDetail
properties_list:
- description: ''
  name: autoResolve
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: secretId
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-pager-duty-incident-detail-schema.json
slug: incident-manager-pager-duty-incident-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-pager-duty-incident-detail-schema.json\",\n  \"title\": \"PagerDutyIncidentDetail\",\n  \"description\": \"Details about the PagerDuty incident associated with an incident created by an Incident Manager response plan.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autoResolve\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether to resolve the PagerDuty incident when you resolve the associated Incident Manager incident.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyIncidentDetailIdString\"\n        },\n        {\n          \"description\": \"The ID of the incident associated with the\
  \ PagerDuty service for the response plan.\"\n        }\n      ]\n    },\n    \"secretId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PagerDutyIncidentDetailSecretIdString\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services Secrets Manager secret that stores your PagerDuty key, either a General Access REST API Key or User Token REST API Key, and other user credentials.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-pager-duty-incident-detail-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: PagerDutyIncidentDetail
---
