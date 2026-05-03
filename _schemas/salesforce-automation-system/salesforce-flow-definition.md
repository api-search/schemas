---
description: Schema for a Salesforce Flow definition record from the Tooling API.
layout: schema
name: Salesforce Flow Definition
properties_list:
- description: Salesforce record ID for the FlowDefinition.
  name: Id
  type: string
- description: Developer API name used to identify the flow programmatically.
  name: ApiName
  type: string
- description: Human-readable label displayed in the Salesforce UI.
  name: Label
  type: string
- description: Optional description of the flow's purpose.
  name: Description
  type: string
- description: Current status of the flow version.
  name: Status
  type: string
- description: The type of flow, determining how it is triggered and used.
  name: ProcessType
  type: string
- description: What event triggers the flow (for record-triggered and scheduled flows).
  name: TriggerType
  type: string
- description: ID of the currently active Flow version.
  name: ActiveVersionId
  type: string
- description: ID of the most recently saved (draft or active) Flow version.
  name: LatestVersionId
  type: string
- description: Package state of the flow.
  name: ManageableState
  type: string
- description: ISO 8601 timestamp when the flow was created.
  name: CreatedDate
  type: string
- description: ISO 8601 timestamp of the last modification.
  name: LastModifiedDate
  type: string
provider_name: Salesforce Automation System
provider_slug: salesforce-automation-system
schema_file: json-schema/salesforce-flow-definition-schema.json
slug: salesforce-flow-definition
source_filename: salesforce-flow-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-automation-system/json-schema/salesforce-flow-definition-schema.json\",\n  \"title\": \"Salesforce Flow Definition\",\n  \"description\": \"Schema for a Salesforce Flow definition record from the Tooling API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID for the FlowDefinition.\"\n    },\n    \"ApiName\": {\n      \"type\": \"string\",\n      \"description\": \"Developer API name used to identify the flow programmatically.\"\n    },\n    \"Label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label displayed in the Salesforce UI.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the flow's purpose.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\"Active\", \"Draft\", \"Obsolete\", \"InvalidDraft\"],\n      \"description\": \"Current status of the flow version.\"\n    },\n    \"ProcessType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Flow\",\n        \"AutoLaunchedFlow\",\n        \"Workflow\",\n        \"CustomEvent\",\n        \"InvocableProcess\",\n        \"LoginFlow\",\n        \"ActionPlan\",\n        \"AppProcess\",\n        \"FieldServiceMobile\",\n        \"FieldServiceWeb\",\n        \"Survey\",\n        \"SurveyEnrich\"\n      ],\n      \"description\": \"The type of flow, determining how it is triggered and used.\"\n    },\n    \"TriggerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RecordBeforeSave\",\n        \"RecordAfterSave\",\n        \"RecordBeforeDelete\",\n        \"Scheduled\",\n        \"PlatformEvent\",\n        null\n      ],\n      \"description\": \"What event triggers the flow (for record-triggered and scheduled flows).\"\n    },\n    \"ActiveVersionId\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"ID of the currently active Flow version.\"\n    },\n    \"LatestVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the most recently saved (draft or active) Flow version.\"\n    },\n    \"ManageableState\": {\n      \"type\": \"string\",\n      \"enum\": [\"installed\", \"installedEditable\", \"unmanaged\", \"released\", \"deleted\", \"deprecated\"],\n      \"description\": \"Package state of the flow.\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the flow was created.\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last modification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation-system/refs/heads/main/json-schema/salesforce-flow-definition-schema.json
tags:
- Approval Process
- Automation
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
title: Salesforce Flow Definition
---
