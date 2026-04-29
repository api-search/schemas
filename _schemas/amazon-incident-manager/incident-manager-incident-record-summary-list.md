---
description: IncidentRecordSummaryList schema
layout: schema
name: IncidentRecordSummaryList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-incident-record-summary-list-schema.json
slug: incident-manager-incident-record-summary-list
source_filename: incident-manager-incident-record-summary-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-record-summary-list-schema.json\",\n  \"title\": \"IncidentRecordSummaryList\",\n  \"description\": \"IncidentRecordSummaryList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"arn\",\n      \"creationTime\",\n      \"impact\",\n      \"incidentRecordSource\",\n      \"status\",\n      \"title\"\n    ],\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of the incident.\"\n          }\n        ]\n      },\n      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n         \
  \ {\n            \"description\": \"The time the incident was created.\"\n          }\n        ]\n      },\n      \"impact\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Impact\"\n          },\n          {\n            \"description\": \"Defines the impact to customers and applications.\"\n          }\n        ]\n      },\n      \"incidentRecordSource\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IncidentRecordSource\"\n          },\n          {\n            \"description\": \"What caused Incident Manager to create the incident.\"\n          }\n        ]\n      },\n      \"resolvedTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time the incident was resolved.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IncidentRecordStatus\"\
  \n          },\n          {\n            \"description\": \"The current status of the incident.\"\n          }\n        ]\n      },\n      \"title\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IncidentTitle\"\n          },\n          {\n            \"description\": \"The title of the incident. This value is either provided by the response plan or overwritten on creation.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Details describing an incident record.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-incident-record-summary-list-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: IncidentRecordSummaryList
---
