---
description: An SSM document configuration for post-launch automation
layout: schema
name: SsmDocument
properties_list:
- description: Name of the SSM action
  name: actionName
  type: string
- description: SSM document name
  name: ssmDocumentName
  type: string
- description: Timeout in seconds
  name: timeoutSeconds
  type: integer
- description: Whether this action must succeed for cutover to proceed
  name: mustSucceedForCutover
  type: boolean
- description: SSM document parameters
  name: parameters
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-ssm-document-schema.json
slug: application-migration-service-ssm-document
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-ssm-document-schema.json\",\n  \"title\": \"SsmDocument\",\n  \"description\": \"An SSM document configuration for post-launch automation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SSM action\"\n    },\n    \"ssmDocumentName\": {\n      \"type\": \"string\",\n      \"description\": \"SSM document name\"\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds\"\n    },\n    \"mustSucceedForCutover\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this action must succeed for cutover to proceed\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"SSM document parameters\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-ssm-document-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: SsmDocument
---
