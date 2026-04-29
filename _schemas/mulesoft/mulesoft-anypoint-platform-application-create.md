---
description: Request body for creating a new CloudHub application
layout: schema
name: ApplicationCreate
properties_list:
- description: Unique domain name for the application
  name: domain
  type: string
- description: Target Mule runtime version
  name: muleVersion
  type: object
- description: CloudHub region to deploy to
  name: region
  type: string
- description: Application properties
  name: properties
  type: object
- description: Enable automatic restart on failure
  name: monitoringAutoRestart
  type: boolean
- description: Enable persistent queues
  name: persistentQueues
  type: boolean
- description: Enable static IP allocation
  name: staticIPsEnabled
  type: boolean
- description: Enable next-generation logging
  name: loggingNgEnabled
  type: boolean
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-application-create-schema.json
slug: mulesoft-anypoint-platform-application-create
source_filename: mulesoft-anypoint-platform-application-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new CloudHub application\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Unique domain name for the application\"\n    },\n    \"muleVersion\": {\n      \"type\": \"object\",\n      \"description\": \"Target Mule runtime version\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"CloudHub region to deploy to\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Application properties\"\n    },\n    \"monitoringAutoRestart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable automatic restart on failure\"\n    },\n    \"persistentQueues\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable persistent queues\"\n    },\n    \"staticIPsEnabled\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Enable static IP allocation\"\n    },\n    \"loggingNgEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable next-generation logging\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-application-create-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: ApplicationCreate
---
