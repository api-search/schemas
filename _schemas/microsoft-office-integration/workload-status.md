---
description: The health status of an Office 365 workload as returned by the Service Communications API current and historical status endpoints.
layout: schema
name: WorkloadStatus
properties_list:
- description: The workload identifier.
  name: Id
  type: string
- description: The workload name.
  name: Workload
  type: string
- description: The date of the status.
  name: StatusDate
  type: string
- description: The display name of the workload.
  name: WorkloadDisplayName
  type: string
- description: The overall status of the workload.
  name: Status
  type: string
- description: List of incident identifiers affecting the workload.
  name: IncidentIds
  type: array
- description: Status of individual features within the workload.
  name: FeatureGroupStatusCollection
  type: array
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
schema_file: json-schema/workload-status.json
slug: workload-status
source_filename: workload-status.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"workload-status.json\",\n  \"title\": \"WorkloadStatus\",\n  \"description\": \"The health status of an Office 365 workload as returned by the Service Communications API current and historical status endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The workload identifier.\"\n    },\n    \"Workload\": {\n      \"type\": \"string\",\n      \"description\": \"The workload name.\"\n    },\n    \"StatusDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date of the status.\"\n    },\n    \"WorkloadDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the workload.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The overall status of the workload.\",\n      \"enum\": [\n        \"ServiceOperational\"\
  ,\n        \"Investigating\",\n        \"ServiceDegradation\",\n        \"ServiceInterruption\",\n        \"RestoringService\",\n        \"ExtendedRecovery\",\n        \"InvestigationSuspended\",\n        \"ServiceRestored\",\n        \"FalsePositive\",\n        \"PostIncidentReportPublished\",\n        \"InformationAvailable\"\n      ]\n    },\n    \"IncidentIds\": {\n      \"type\": \"array\",\n      \"description\": \"List of incident identifiers affecting the workload.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"FeatureGroupStatusCollection\": {\n      \"type\": \"array\",\n      \"description\": \"Status of individual features within the workload.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Feature\": {\n            \"type\": \"string\",\n            \"description\": \"The feature identifier.\"\n          },\n          \"FeatureGroupDisplayName\": {\n            \"type\": \"string\",\n            \"\
  description\": \"The display name of the feature.\"\n          },\n          \"FeatureStatus\": {\n            \"type\": \"string\",\n            \"description\": \"The status of the feature.\",\n            \"enum\": [\n              \"ServiceOperational\",\n              \"Investigating\",\n              \"ServiceDegradation\",\n              \"ServiceInterruption\",\n              \"RestoringService\",\n              \"ExtendedRecovery\",\n              \"InvestigationSuspended\",\n              \"ServiceRestored\",\n              \"FalsePositive\",\n              \"PostIncidentReportPublished\",\n              \"InformationAvailable\"\n            ]\n          }\n        },\n        \"required\": [\"Feature\", \"FeatureGroupDisplayName\", \"FeatureStatus\"]\n      }\n    }\n  },\n  \"required\": [\"Id\", \"Workload\", \"StatusDate\", \"WorkloadDisplayName\", \"Status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/json-schema/workload-status.json
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
title: WorkloadStatus
---
