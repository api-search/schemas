---
description: Represents an integration event record within the Workday Integrations system, tracking the execution status and details of integration runs.
layout: schema
name: Integration Event
properties_list:
- description: The unique Workday identifier for the integration event
  name: id
  type: string
- description: The display name of the integration event
  name: descriptor
  type: string
- description: The integration system that was executed
  name: integrationSystem
  type: object
- description: The execution status of the integration
  name: status
  type: string
- description: The date and time the integration started
  name: startDateTime
  type: string
- description: The date and time the integration completed
  name: endDateTime
  type:
  - string
  - 'null'
- description: The number of records successfully processed
  name: recordsProcessed
  type: integer
- description: The number of records that failed processing
  name: recordsFailed
  type: integer
- description: The user or system that initiated the integration
  name: initiatedBy
  type: object
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-integration-event-schema.json
slug: workday-integration-integration-event
source_filename: workday-integration-integration-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/integrationEvent\",\n  \"title\": \"Integration Event\",\n  \"description\": \"Represents an integration event record within the Workday Integrations system, tracking the execution status and details of integration runs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the integration event\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the integration event\"\n    },\n    \"integrationSystem\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The integration system that was executed\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Completed\", \"Failed\", \"In_Progress\", \"Cancelled\"],\n      \"description\": \"The execution status of the integration\"\
  \n    },\n    \"startDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the integration started\"\n    },\n    \"endDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the integration completed\"\n    },\n    \"recordsProcessed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records successfully processed\"\n    },\n    \"recordsFailed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records that failed processing\"\n    },\n    \"initiatedBy\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The user or system that initiated the integration\"\n    }\n  },\n  \"required\": [\"id\", \"integrationSystem\", \"status\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"\
  string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-integration-event-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Integration Event
---
