---
description: Details about what caused the incident to be created in Incident Manager.
layout: schema
name: TriggerDetails
properties_list:
- description: ''
  name: rawData
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: timestamp
  type: object
- description: ''
  name: triggerArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-trigger-details-schema.json
slug: incident-manager-trigger-details
source_filename: incident-manager-trigger-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-trigger-details-schema.json\",\n  \"title\": \"TriggerDetails\",\n  \"description\": \"Details about what caused the incident to be created in Incident Manager.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rawData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawData\"\n        },\n        {\n          \"description\": \"Raw data passed from either Amazon EventBridge, Amazon CloudWatch, or Incident Manager when an incident is created.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentSource\"\n        },\n        {\n          \"description\": \"Identifies the service that sourced the event. All events sourced from within Amazon Web Services begin with \\\
  \"<code>aws.</code>\\\" Customer-generated events can have any value here, as long as it doesn't begin with \\\"<code>aws.</code>\\\" We recommend the use of Java package-name style reverse domain-name strings. \"\n        }\n      ]\n    },\n    \"timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the incident was detected.\"\n        }\n      ]\n    },\n    \"triggerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the source that detected the incident.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-trigger-details-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: TriggerDetails
---
