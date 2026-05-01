---
description: Details about what created the incident record and when it was created.
layout: schema
name: IncidentRecordSource
properties_list:
- description: ''
  name: createdBy
  type: object
- description: ''
  name: invokedBy
  type: object
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: source
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-incident-record-source-schema.json
slug: incident-manager-incident-record-source
source_filename: incident-manager-incident-record-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-record-source-schema.json\",\n  \"title\": \"IncidentRecordSource\",\n  \"description\": \"Details about what created the incident record and when it was created.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The principal that started the incident.\"\n        }\n      ]\n    },\n    \"invokedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServicePrincipal\"\n        },\n        {\n          \"description\": \"The service principal that assumed the role specified in <code>createdBy</code>. If no service principal assumed the role this will be left blank.\"\n        }\n      ]\n\
  \    },\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The resource that caused the incident to be created.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentSource\"\n        },\n        {\n          \"description\": \"The service that started the incident. This can be manually created from Incident Manager, automatically created using an Amazon CloudWatch alarm, or Amazon EventBridge event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createdBy\",\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-record-source-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: IncidentRecordSource
---
