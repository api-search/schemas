---
description: ListIncidentRecordsOutput schema
layout: schema
name: ListIncidentRecordsOutput
properties_list:
- description: ''
  name: incidentRecordSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-incident-records-output-schema.json
slug: incident-manager-list-incident-records-output
source_filename: incident-manager-list-incident-records-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-incident-records-output-schema.json\",\n  \"title\": \"ListIncidentRecordsOutput\",\n  \"description\": \"ListIncidentRecordsOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incidentRecordSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentRecordSummaryList\"\n        },\n        {\n          \"description\": \"The details of each listed incident record.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentRecordSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-incident-records-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: ListIncidentRecordsOutput
---
