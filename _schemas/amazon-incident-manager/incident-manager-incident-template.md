---
description: Basic details used in creating a response plan. The response plan is then used to create an incident record.
layout: schema
name: IncidentTemplate
properties_list:
- description: ''
  name: dedupeString
  type: object
- description: ''
  name: impact
  type: object
- description: ''
  name: incidentTags
  type: object
- description: ''
  name: notificationTargets
  type: object
- description: ''
  name: summary
  type: object
- description: ''
  name: title
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-incident-template-schema.json
slug: incident-manager-incident-template
source_filename: incident-manager-incident-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-template-schema.json\",\n  \"title\": \"IncidentTemplate\",\n  \"description\": \"Basic details used in creating a response plan. The response plan is then used to create an incident record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dedupeString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedupeString\"\n        },\n        {\n          \"description\": \"Used to stop Incident Manager from creating multiple incident records for the same incident. \"\n        }\n      ]\n    },\n    \"impact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Impact\"\n        },\n        {\n          \"description\": \"The impact of the incident on your customers and applications. \"\n        }\n      ]\n   \
  \ },\n    \"incidentTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags to assign to the template. When the <code>StartIncident</code> API action is called, Incident Manager assigns the tags specified in the template to the incident.\"\n        }\n      ]\n    },\n    \"notificationTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetSet\"\n        },\n        {\n          \"description\": \"The Amazon SNS targets that are notified when updates are made to an incident.\"\n        }\n      ]\n    },\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentSummary\"\n        },\n        {\n          \"description\": \"The summary of the incident. The summary is a brief synopsis of what occurred, what's currently happening, and context.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTitle\"\n        },\n        {\n          \"description\": \"The title of the incident. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"impact\",\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-template-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: IncidentTemplate
---
