---
description: A lifecycle action hook for a source server
layout: schema
name: SourceServerAction
properties_list:
- description: Action ID
  name: actionID
  type: string
- description: Action name
  name: actionName
  type: string
- description: Whether the action is active
  name: active
  type: boolean
- description: Action category
  name: category
  type: string
- description: Action description
  name: description
  type: string
- description: SSM document identifier
  name: documentIdentifier
  type: string
- description: SSM document version
  name: documentVersion
  type: string
- description: External parameters for the action
  name: externalParameters
  type: object
- description: Whether action must succeed for cutover
  name: mustSucceedForCutover
  type: boolean
- description: Execution order
  name: order
  type: integer
- description: Action parameters
  name: parameters
  type: object
- description: Timeout in seconds
  name: timeoutSeconds
  type: integer
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-source-server-action-schema.json
slug: application-migration-service-source-server-action
source_filename: application-migration-service-source-server-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-source-server-action-schema.json\",\n  \"title\": \"SourceServerAction\",\n  \"description\": \"A lifecycle action hook for a source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionID\": {\n      \"type\": \"string\",\n      \"description\": \"Action ID\"\n    },\n    \"actionName\": {\n      \"type\": \"string\",\n      \"description\": \"Action name\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the action is active\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Action category\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Action description\"\n    },\n    \"documentIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"\
  SSM document identifier\"\n    },\n    \"documentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"SSM document version\"\n    },\n    \"externalParameters\": {\n      \"type\": \"object\",\n      \"description\": \"External parameters for the action\"\n    },\n    \"mustSucceedForCutover\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether action must succeed for cutover\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Execution order\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Action parameters\"\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-source-server-action-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: SourceServerAction
---
