---
description: Schema for a Salesforce Flow definition object representing an automation process.
layout: schema
name: Salesforce Flow Definition
properties_list:
- description: Salesforce record ID for the Flow
  name: Id
  type: string
- description: API name of the Flow (unique identifier within the org)
  name: ApiName
  type: string
- description: Display label of the Flow shown in the UI
  name: Label
  type: string
- description: Description of the Flow's purpose
  name: Description
  type: string
- description: Type of Flow automation process
  name: ProcessType
  type: string
- description: Activation status of the Flow
  name: Status
  type: string
- description: Version number of the flow
  name: VersionNumber
  type: integer
- description: Run mode for the flow
  name: RunInMode
  type: string
- description: Timestamp when the flow was created
  name: CreatedDate
  type: string
- description: Timestamp when the flow was last modified
  name: LastModifiedDate
  type: string
- description: Salesforce ID of the user who created the flow
  name: CreatedById
  type: string
- description: Salesforce ID of the user who last modified the flow
  name: LastModifiedById
  type: string
provider_name: Salesforce Flow
provider_slug: salesforce-flow
schema_file: json-schema/salesforce-flow-flow-definition-schema.json
slug: salesforce-flow-flow-definition
source_filename: salesforce-flow-flow-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-flow/blob/main/json-schema/salesforce-flow-flow-definition-schema.json\",\n  \"title\": \"Salesforce Flow Definition\",\n  \"description\": \"Schema for a Salesforce Flow definition object representing an automation process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID for the Flow\",\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"ApiName\": {\n      \"type\": \"string\",\n      \"description\": \"API name of the Flow (unique identifier within the org)\",\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9_]*$\"\n    },\n    \"Label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label of the Flow shown in the UI\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the Flow's purpose\"\
  \n    },\n    \"ProcessType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of Flow automation process\",\n      \"enum\": [\n        \"Flow\",\n        \"AutoLaunchedFlow\",\n        \"Workflow\",\n        \"InvocableProcess\",\n        \"CustomEvent\",\n        \"FieldServiceMobile\",\n        \"FieldServiceWeb\",\n        \"Survey\",\n        \"SurveyEnrich\",\n        \"Orchestrator\",\n        \"ContactRequestFlow\",\n        \"RoutingFlow\",\n        \"TransactionSecurityFlow\",\n        \"ServiceCatalogItemFlow\"\n      ]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Activation status of the Flow\",\n      \"enum\": [\"Active\", \"Obsolete\", \"Draft\", \"InvalidDraft\"]\n    },\n    \"VersionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the flow\",\n      \"minimum\": 1\n    },\n    \"RunInMode\": {\n      \"type\": \"string\",\n      \"description\": \"Run mode for the flow\",\n      \"\
  enum\": [\"DefaultMode\", \"SystemModeWithSharing\", \"SystemModeWithoutSharing\"]\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the flow was created\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the flow was last modified\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the user who created the flow\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the user who last modified the flow\"\n    }\n  },\n  \"required\": [\"Id\", \"ApiName\", \"Label\", \"ProcessType\", \"Status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-flow/refs/heads/main/json-schema/salesforce-flow-flow-definition-schema.json
tags:
- Automation
- Business Process
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
title: Salesforce Flow Definition
---
